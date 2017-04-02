In software development, there are certain design problems that crop up repeatedly.    

<panel header="Some examples of recurring design problems :zero:" type="seamless" expandable>

* An example problem about software architecture: what is the best <trigger for="pop:architecture">architecture</trigger> for a given type of system?
* An example problem about the interaction between classes: how to lower the 
  <trigger for="tt:coupling">coupling</trigger> between  `UI` and `Logic` classes ?
* <panel header="Some more examples :zero: " expandable type="seamless">

  * Another example
  * One more example about <trigger for="tt:coupling">coupling</trigger>

  </panel>
</panel><br>

After repeated attempts at solving such design problems, better solutions are discovered and refined 
over time. These solutions are collectively known as<trigger trigger="click" for="modal:gofbook"> _design patterns_</trigger>, a term popularized by the seminal _Gang of Four book_.

<panel header="More about Gang of Four Book :zero:" type="seamless" expandable>
  <div class="pull-right">
  <pic src="introduction/book-designpatterns.jpg" width="200px">GoF Book Cover </pic>
  </div>

  **Design Patterns: Elements of Reusable Object-Oriented Software** by the four authors Eric Gamma, Richard Helm, Ralph Johnson and John Vlissides is also known as  the _Gang of Four_ book or _GoF book_. It is also probably the  most famous book about design patterns.

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

**Test your understanding:**

* Definition of a _design pattern_
  <morph title="Q1  :one:" src="Q-Essay-WhatIsAPattern.md" />
  <morph title="Q1a :zero:" src="Q-Essay-WhatIsAPattern.md" />
  <morph title="Q1b :zero:" src="Q-Essay-WhatIsAPattern.md" />
* Attributes of a _design pattern_
  <morph title="Q2  :one: " src="Q-Tick-PatternAttributes.md" />
  <morph title="Q2a :zero: " src="Q-Tick-PatternAttributes.md" />

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

  <include src="GoF.md" />

</modal>