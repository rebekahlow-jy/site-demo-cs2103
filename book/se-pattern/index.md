<link rel="stylesheet" href="{{baseUrl}}/css/main.css">
<link rel="stylesheet" href="{{baseUrl}}/css/textbook.css">

<include src="../../common/header.md" />

<div class="website-content">

# Software Design Patterns

<div v-closeable alt="definition">

<panel header="**What are _Software Design Patterns_?** :one:" expandable type="seamless">
  <include src="introduction/index.md" />
</panel>

</div>
<!-- --------------------------------------------------------------------------------------------------------- -->
<div v-closeable alt="format"><hr>


%%Because design patterns document design solutions meant to be shared, they are usually documented in a certain format.%%

<panel header="**Format for documenting a design pattern** :one:" expandable type="seamless">
  <include src="format/index.md" />
</panel>

</div>
<!-- --------------------------------------------------------------------------------------------------------- -->
<div v-closeable alt="examples"><hr>

%%There are many design patterns. Given below are some better known ones.%%

<Panel header="**Singleton pattern** :one:" expandable type="seamless">
  <include src="singleton/index.md" /><hr>
</Panel>
<Panel header="**Façade pattern** :one:" expandable type="seamless">
  <include src="facade/index.md" />
</Panel>

<Panel header="**Command pattern** :one:" expandable type="seamless">
  <include src="command/index.md" />
</Panel>

<Panel header="**Mode-View-Controller pattern** :two:" expandable type="seamless">
  <include src="mvc/index.md" />
</Panel>

<Panel header="**Observer pattern** :two:" expandable type="seamless">
  <include src="observer/index.md" />
</Panel>

<Panel header="**Abstraction occurrence pattern** :three:" expandable type="seamless">
  <include src="abstraction-occurrence/index.md" />
</Panel>

</div>
<!-- --------------------------------------------------------------------------------------------------------- -->
<div v-closeable alt="case study"><hr>


%%While we can learn each design pattern in isolation, in practice they are often applied in combination. Let us look at a case study that combines several design patterns.%%

<Panel header="**Case Study** :two:" expandable type="seamless">
  <include src="case-study/index.md" />
</Panel>

</div>
<!-- --------------------------------------------------------------------------------------------------------- -->
<div v-closeable alt="patterns beyond software design"><hr>


%%Patterns go beyond software design. In fact, they did not even originate in software design.%%

<Panel header="**How patterns originated in building architecture domain** :zero:" expandable type="seamless">
  <include src="beyond/index.md" />
</Panel>
<Panel header="**Patterns from other domains** :three:" expandable type="seamless">
  <include src="beyond/index.md" />
</Panel>

</div>
<!-- --------------------------------------------------------------------------------------------------------- -->
<div v-closeable alt="extras"><hr>

<panel header=":paperclip: Extras" expandable type="seamless">

  <panel header=":bulb: Test your knowledge" expandable type="seamless">
    <morph title="Q1a :one:" src="./examples/e1.md"></morph>
    <morph title="Q1b :zero:" src="./examples/e2.md"></morph>
    <morph title="Q1c :zero:" src="./examples/e3.md"></morph><br/>
    <morph title="Q2a :one:" src="./examples/e4.md"></morph>
    <morph title="Q2b :zero:" src="./examples/e5.md"></morph>
  </panel>

</panel>

</div>

</div>

