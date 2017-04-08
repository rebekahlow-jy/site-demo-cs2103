> Some software design problems crop up repeatedly. After repeated attempts at solving such design problems, better solutions are discovered and refined over time. These solutions are collectively known as _design patterns_, a term popularized by the seminal <trigger trigger="click" for="modal:gofbook">_Gang of Four book_</trigger>.   

<panel header="Some examples of recurring design problems :zero:" type="seamless" expandable>

* An example problem about software architecture: what is the best <trigger for="pop:architecture">architecture</trigger> for a given type of system?
* An example problem about the interaction between classes: how to lower the 
  <trigger for="tt:coupling">coupling</trigger> between  `UI` and `Logic` classes ?
* <panel header="Some more examples :zero: " expandable type="seamless">

  * Another example
  * One more example about <trigger for="tt:coupling">coupling</trigger>

  </panel>
</panel><br>

<panel header="More about Gang of Four Book :zero:" type="seamless" expandable>
  <div class="pull-right">
  <pic src="introduction/book-designpatterns.jpg" width="200px">GoF Book Cover </pic>
  </div>

  **Design Patterns: Elements of Reusable Object-Oriented Software** by the four authors Eric Gamma, Richard Helm, Ralph Johnson and John Vlissides is also known as  the _Gang of Four_ book or _GoF book_. It is also probably the  most famous book about design patterns.

</panel><br>

<tip-box type="info">

**Software Design Pattern** :
<include src="../../common/Definitions.md#def-se-design-pattern"/>

</tip-box>


Because design patterns document design solutions meant to be shared, they are usually documented in a certain format.

<panel header="Format for documenting a desing pattern :one:" expandable type="seamless" is-open="true">

<div class="pull-right" v-closeable alt="comic">
 <img src="http://www.topswagcode.com/content/images/2016/02/developer-patterns.jpg" width="250"/>
</div>

The common format to describe a pattern consists of the following components: 
* **Context**: The situation or scenario where the design problem is encountered.
* **Problem**: The main difficulty to be resolved. The criteria for a good solution are also identified to evaluate solutions.
* **Solution**: The core of the solution. It is important to note that the solution presented only includes the most general constraints, which may need further refinement for a specific context.
* **Anti-patterns** (optional): Commonly used solutions, which are usually incorrect and/or inferior to the Design Pattern.
* **Consequences** (optional): Identifying the pros and cons of applying the pattern.
* **Other useful information** (optional): Code examples, known uses, other related patterns, etc.

</panel>

<panel header="Above description is too abstract? Here is an illustrative example :zero:" expandable type="seamless">
  <include src="../singleton/index.md" />
</panel><br>

<panel header=":mortar_board: Learning Outcomes" expandable type="seamless">

* :one: Able to explain what is a design pattern
* :one: Able to describe distinguishing characteristics of a design pattern

</panel>

<panel header=":bulb: Test your knowledge" expandable type="seamless">

:question: Definition of a _design pattern_
  <morph title="Q1  :one:" src="Q-Essay-WhatIsAPattern.md" />
  <morph title="Q1a :zero:" src="Q-Essay-WhatIsAPattern.md" />
  <morph title="Q1b :zero:" src="Q-Essay-WhatIsAPattern.md" /><br>
:question: Attributes of a _design pattern_
  <morph title="Q2  :one: " src="Q-Tick-PatternAttributes.md" />
  <morph title="Q2a :zero: " src="Q-Tick-PatternAttributes.md" />
  
</panel>

<panel header=":pencil: Apply your knowledge" expandable type="seamless">

* :one: Do the exercise given in [SE-EDU: Addressbook Level 4: Apply Design Patterns](https://github.com/se-edu/addressbook-level4/blob/master/docs/LearningOutcomes.md#apply-design-patterns-lo-designpatterns)

</panel>

<panel header=":package: Resources" expandable type="seamless">

* :one: GoF Book
* :zero: Resource 2
* :two: Resrouce 3

</panel>

<panel header="::laughing:: Humor" expandable type="seamless">

<img src="http://www.topswagcode.com/content/images/2016/02/developer-patterns.jpg" width="250"/>

</panel>

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