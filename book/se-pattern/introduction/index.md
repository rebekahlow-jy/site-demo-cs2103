In software development, there are certain design problems that crop up repeatedly.    

* An example problem about software architecture: what is the best <trigger for="pop:architecture">architecture</trigger> for a given type of system?
* An example problem about the interaction between classes: how to lower the 
  <trigger for="tt:coupling">coupling</trigger> between  `UI` and `Logic` classes ?
* <panel header="Some more examples :zero: " expandable type="seamless">

  * Another example
  * One more example about <trigger for="tt:coupling">coupling</trigger>

  </panel>

After repeated attempts at solving such design problems, better solutions are discovered and refined 
over time. These solutions are collectively known as<trigger trigger="click" for="modal:gofbook"> _design patterns_</trigger>, a term popularized by the seminal _Gang of Four book_.

<panel header="More about Gang of Four(GoF) Book :zero:" type="seamless" expandable>
  <div class="pull-right">
  <pic src="introduction/book-designpatterns.jpg" width="200px">GoF Book Cover </pic>
  </div>
  
  The term _design patterns_ was popularized by the seminal book 
  *Design Patterns: Elements of Reusable Object-Oriented Software* also known as  the so-called _Gang of Four_ (GoF) book by Eric Gamma, Richard Helm, Ralph Johnson and John Vlissides.
  
  The authors of the DesignPatternsBook came to be known as the "Gang of Four." The name of the book ("Design Patterns: Elements of Reusable Object-Oriented Software") is too long for e-mail, so "book by the gang of four" became a shorthand name for it. After all, it isn't the ONLY book on patterns. That got shortened to "GOF book", which is pretty cryptic the first time you hear it.
  
</panel><br>

<tip-box type="info">

**Software Design Pattern** :
<include src="../../common/Definitions.md#def-se-design-pattern" />

</tip-box>

<panel header="Documenting a design pattern :one:" expandable type="seamless" is-open="true">

The common format to describe a pattern consists of the following components: 
* **Context**: The situation or scenario where the design problem is encountered.
* **Problem**: The main difficulty to be resolved. The criteria for a good solution are also identified to evaluate solutions.
* **Solution**: The core of the solution. It is important to note that the solution presented only includes the most general constraints, which may need further refinement for a specific context.
* **Anti-patterns** (optional): Commonly used solutions, which are usually incorrect and/or inferior to the Design Pattern.
* **Consequences** (optional): Identifying the pros and cons of applying the pattern.
* **Other useful information** (optional): Code examples, known uses, other related patterns, etc.

<hr>

</panel>

<panel header="Above description is too abstract? Here is an illustrative example :zero:" expandable type="seamless">
  <include src="../singleton/index.md" />
</panel><br>

**Self-test questions:**

<morph title="Q1" src="Q-Essay-WhatIsAPattern.md" />

<!-- additional info -->

<popover id="pop:architecture">
  <div slot="content">
  
  _**Software architecture**_ :
  
  <include src="../../common/Definitions.md#def-architecture" />

  </div>
</popover>

<tooltip id="tt:coupling">
  <div slot="content">
  
  <include src="../../common/Definitions.md#def-coupling" />

  </div>
</tooltip>

<modal title="**GoF Book** :zero:" id="modal:gofbook">

  <pic src="introduction/book-designpatterns.jpg" width="400px" />
  
  The authors of the DesignPatternsBook came to be known as the "Gang of Four." The name of the book ("Design Patterns: Elements of Reusable Object-Oriented Software") is too long for e-mail, so "book by the gang of four" became a shorthand name for it. After all, it isn't the ONLY book on patterns. That got shortened to "GOF book", which is pretty cryptic the first time you hear it. 
  
  <panel header="An example pattern from the book: Singleton :one: " expandable type="seamless">
    <include src="../singleton/index.md" />
  </panel>

</modal>