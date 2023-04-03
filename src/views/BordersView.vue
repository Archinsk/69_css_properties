<template>
  <div>
    <h3>Borders</h3>
    <div class="buttons">
      <button>default</button>
      <button class="btn-transparent">Button</button>
      <button class="btn-transparent btn-bordered">Button</button>
      <button class="btn-transparent btn-only-left-border">Button</button>
      <button class="btn-transparent btn-only-left-border-facet">Button</button>
      <button class="btn-transparent btn-bordered rounded">Button</button>
      <button class="btn-transparent btn-only-left-border rounded">
        Button
      </button>
      <button class="btn-transparent btn-only-left-border-facet rounded">
        Button
      </button>
      <h4>
        border-style (border-top-style, border-right-style, border-bottom-style,
        border-left-style)
      </h4>
      <div class="example-group">
        <div class="display-flex align-items-center">
          <div class="example-brick"></div>
          <div>default (without border-style)</div>
        </div>
        <div class="display-flex align-items-center">
          <div class="example-brick border-style-none"></div>
          <div>border-style: none;</div>
        </div>
        <div class="display-flex align-items-center">
          <div class="example-brick border-style-hidden"></div>
          <div>border-style: hidden;</div>
        </div>
        <div class="display-flex align-items-center">
          <div class="example-brick border-style-dotted"></div>
          <div>border-style: dotted;</div>
        </div>
        <div class="display-flex align-items-center">
          <div class="example-brick border-style-dashed"></div>
          <div>border-style: dashed;</div>
        </div>
        <div class="display-flex align-items-center">
          <div class="example-brick border-style-solid"></div>
          <div>border-style: solid;</div>
        </div>
        <div class="display-flex align-items-center">
          <div class="example-brick border-style-double"></div>
          <div>border-style: double;</div>
        </div>
        <div class="display-flex align-items-center">
          <div class="example-brick border-style-groove"></div>
          <div>border-style: groove;</div>
        </div>
        <div class="display-flex align-items-center">
          <div class="example-brick border-style-ridge"></div>
          <div>border-style: ridge;</div>
        </div>
        <div class="display-flex align-items-center">
          <div class="example-brick border-style-inset"></div>
          <div>border-style: inset;</div>
        </div>
        <div class="display-flex align-items-center">
          <div class="example-brick border-style-outset"></div>
          <div>border-style: outset;</div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "BordersView",
};
</script>

<style scoped lang="scss">
.buttons > :not(:last-child) {
  margin-bottom: 0.5rem;
}

.btn-transparent {
  display: block;
  background-color: transparent;
}

.btn-bordered {
  border: solid 3px blue;
}

.btn-only-left-border {
  border-color: blue;
  border-width: 0;
  border-left-width: 6px;
}

.btn-only-left-border-facet {
  border-color: transparent;
  border-left-color: red;
  border-width: 0;
  border-width: 6px;
}

.rounded {
  border-radius: 6px;
}

.example-group {
  & > :not(:last-child) {
    margin-bottom: 0.5rem;
  }

  .example-brick {
    background-color: lightgrey;
    width: 5rem;
    height: 2rem;
    margin-right: 1rem;
  }
}

.display-flex {
  display: flex;
}

.align-items-center {
  align-items: center;
}

.border-style-none {
  border-style: none;
}
.border-style-hidden {
  border-style: hidden;
}
.border-style-dotted {
  border-style: dotted;
}

.border-style-dashed {
  border-style: dashed;
}
.border-style-solid {
  border-style: solid;
}
.border-style-double {
  border-style: double;
}
.border-style-groove {
  border-style: groove;
}
.border-style-ridge {
  border-style: ridge;
}
.border-style-inset {
  border-style: inset;
}
.border-style-outset {
  border-style: outset;
}
</style>
