### Patterns

In software development, there are certain problems that crop up repeatedly.    

* An example problem about software architecture: what is the best architecture for a given type of system?
* An example problem about the interaction between classes: how to lower the coupling between UI and Logic classes?    

After repeated attempts at solving such problems, better solutions are discovered and refined over time. These solutions are collectively known as *patterns*, a term popularized by the seminal book *Design Patterns: Elements of Reusable Object-Oriented Software* by the so-called “Gang of Four” (GoF): Eric Gamma, Richard Helm, Ralph Johnson and John Vlissides.

<div class="center-block text-center" v-closeable alt="Show book cover">
<pic src="introduction/book-designpatterns.jpg" width="400px">

The famous Design Patterns book by **GoF** 

</pic>
</div>

Instead of listing a large number of patterns, this handout attempts to guide the reader on understanding patterns as a general concept by referring to a few representative examples to illustrate the concept of patterns. This handout focuses more on patterns in the area of software design (i.e. design patterns). Having understood the general idea of patterns, the reader should be able to pick up more patterns from other resources.

The common format to describe a pattern consists of the following components:
* **Context**: The situation or scenario where the design problem is encountered.
* **Problem**: The main difficulty to be resolved. The criteria for a good solution are also identified to evaluate solutions.
* **Solution**: The core of the solution. It is important to note that the solution presented only includes the most general constraints, which may need further refinement for a specific context.
* **Anti-patterns** (optional): Commonly used solutions, which are usually incorrect and/or inferior to the Design Pattern.
* **Consequences** (optional): Identifying the pros and cons of applying the pattern.
* **Other useful information** (optional): Code examples, known uses, other related patterns, etc.