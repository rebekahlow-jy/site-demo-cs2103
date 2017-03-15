### Singleton Pattern

#### Context
In most systems, it is common to restrict the number of instantiated 
objects of certain classes to just **one** (e.g. the main controller class 
of the system). These single instances are commonly known as *singletons*.

#### Problem
Prohibit the instantiation of more than one object from a singleton class, with the single instance easily shared among those who need it.

#### Solution
The key insight of the solution is that the *constructor* of the singleton class cannot be *public*. Since a *public constructor* will allow others to instantiate the class at will, 
a *private constructor* should be used instead. In addition, a public method is provided to access the *single* instance. This solution is described below.

<img class="center-block" src="singleton/solution.png">

As shown, the solution makes the constructor private (note the “-“ visibility marker for the constructor), 
which prevents instantiation from outside the class. 
The single instance of the singleton class is maintained by a private class-level variable. 
Access to this object is provided by a public class-level operation getInstance(). 
In the skeleton code above, `getInstance()` instantiates a single copy of the singleton class when it is executed for the first time. 
Subsequent calls to this operation return the single instance of the class.

#### Code Example
<tabs>
<tab header="Java">

```java
public class ClassicSingleton {
   private static ClassicSingleton instance = null;
   private ClassicSingleton() {
      // Exists only to defeat instantiation.
   }
   public static ClassicSingleton getInstance() {
      if(instance == null) {
         instance = new ClassicSingleton();
      }
      return instance;
   }
}
```

</tab>
<tab header="C++">

```c++
class GlobalClass
{
    int m_value;
    static GlobalClass *s_instance;
    GlobalClass(int v = 0)
    {
        m_value = v;
    }
  public:
    int get_value()
    {
        return m_value;
    }
    void set_value(int v)
    {
        m_value = v;
    }
    static GlobalClass *instance()
    {
        if (!s_instance)
          s_instance = new GlobalClass;
        return s_instance;
    }
};
```

</tab>
</tabs>

#### Exercise
<morph title="Question 1">
<Question>

Which of the following is an ideal situation for using Singleton pattern?

- ( ) Utility methods used by many class in the application. 
- ( ) A database manager shared by different component of the application.
- ( ) A constant String defined in every controller.  

<div slot="answer">

- ( ) Utility methods used by many class in the application. 
- (X) Database manager shared by different component of the application.
- ( ) A constant String defined in every controller.

Database is a shared resources here, and by using singleton pattern, we have better control
over the database operations.

</div>
</Question>

</morph>