<link rel="stylesheet" href="{{baseUrl}}/css/main.css">
<link rel="stylesheet" href="{{baseUrl}}/css/textbook.css">

<include src="../../common/header.md" />

<div class="website-content">

# Software Design Patterns

<div v-closeable alt="definition">

<panel header="**What are _Software Design Patterns_?** :one:" type="seamless">
  <include src="introduction/index.md" />
</panel>

</div>
<!-- --------------------------------------------------------------------------------------------------------- -->
<div v-closeable alt="format"><hr>


%%Because design patterns document design solutions meant to be shared, they are usually documented in a certain format.%%

<panel header="**Format for documenting a design pattern** :one:" type="seamless">
  <include src="format/index.md" />
</panel>

</div>
<!-- --------------------------------------------------------------------------------------------------------- -->
<div v-closeable alt="examples"><hr>

%%There are many design patterns. Given below are some better known ones.%%

<Panel header="**Singleton pattern** :one:" type="seamless">
  <include src="singleton/index.md#main" /><hr>
</Panel>
<Panel header="**Façade pattern** :one:" type="seamless">
  <include src="facade/index.md" />
</Panel>

<Panel header="**Command pattern** :one:" type="seamless">
  <include src="command/index.md" />
</Panel>

<Panel header="**Mode-View-Controller pattern** :two:" type="seamless">
  <include src="mvc/index.md" />
</Panel>

<Panel header="**Observer pattern** :two:" type="seamless">
  <include src="observer/index.md" />
</Panel>

<Panel header="**Abstraction occurrence pattern** :three:" type="seamless">
  <include src="abstraction-occurrence/index.md" />
</Panel>

</div>
<!-- --------------------------------------------------------------------------------------------------------- -->
<div v-closeable alt="case study"><hr>


%%While we can learn each design pattern in isolation, in practice they are often applied in combination. Let us look at a case study that combines several design patterns.%%

<Panel header="**Case Study** :two:" type="seamless">
  <include src="case-study/index.md" />
</Panel>

</div>
<!-- --------------------------------------------------------------------------------------------------------- -->
<div v-closeable alt="patterns beyond software design"><hr>


%%Patterns go beyond software design. In fact, they did not even originate in software design.%%

<Panel header="**How patterns originated in building architecture domain** :zero:" type="seamless">
  <include src="beyond/index.md" />
</Panel>
<Panel header="**Patterns from other domains** :three:" type="seamless">
  <include src="beyond/index.md" />
</Panel>

</div>
<!-- --------------------------------------------------------------------------------------------------------- -->
<div v-closeable alt="extras"><hr>

<panel header=":paperclip: Extras" type="seamless">

  <panel header=":bulb: Test your knowledge" type="seamless">
    <panel header="Q1a :one:" src="./examples/e1.md" minimized></panel>
    <panel header="Q1b :zero:" src="./examples/e2.md" minimized></panel>
    <panel header="Q1c :zero:" src="./examples/e3.md" minimized></panel><br/>
    <panel header="Q2a :one:" src="./examples/e4.md" minimized></panel>
    <panel header="Q2b :zero:" src="./examples/e5.md" minimized></panel>
  </panel>

</panel>

</div>

</div>
