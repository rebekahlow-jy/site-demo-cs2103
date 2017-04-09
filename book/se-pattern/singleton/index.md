### Singleton Pattern :one:

<div class="pull-right" v-closeable alt="Read lecture slides online">

<iframe src='https://onedrive.live.com/embed?cid=A5AF047C4CAD67AB&resid=A5AF047C4CAD67AB%212074&authkey=&em=2&wdAr=1.3333333333333333' width='350px' height='286px' frameborder='0'>This is an embedded <a target='_blank' href='https://office.com'>Microsoft Office</a> presentation, powered by <a target='_blank' href='https://office.com/webapps'>Office Online</a>.</iframe>

</div>

#### Context
Creating more than one instance of a certain class is undesirable due to some reason <morph title="Examples"> * Example 1 * Example 2 </morph>. If multiple <trigger for="pop:client-code">clients</trigger> need to interact with an instance of the said class, they should share the same single instance. Such a single instance is commonly known as a *singleton*.


#### Problem
Normally, any client can instantiate a class by calling the constructor. This means we can end up with multiple instances of the class in concern.


#### Solution
Make the *constructor* of the singleton class `private`. Provide a `public` method to access the *singleton* instance.

<img class="center-block" src="singleton/solution.png">

As shown, the solution makes the constructor private (note the “-“ visibility marker for the constructor), which prevents instantiation from outside the class. The single instance of the singleton class is maintained by a private class-level variable. Access to this object is provided by a public class-level operation `getInstance()`. In the skeleton code above, `getInstance()` instantiates a single copy of the singleton class when it is executed for the first time. Subsequent calls to this operation return the single instance of the class.

<div v-closeable alt="Read lecture slides online">

@[powerpoint](https://onedrive.live.com/embed?cid=A5AF047C4CAD67AB&resid=A5AF047C4CAD67AB%212070&authkey=&em=2)

</div>

<div v-closeable alt="code examples">

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
</div>

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

<!-- additional info ------------------------------------------------------------------------------------ -->

<tooltip id="pop:client-code">
  <div slot="content">
    <include src="../../common/Definitions.md#def-client-code" />
  </div>
</tooltip>