<template>
  <div id="borders">
    <h3>Borders</h3>
    <h4>
      1. border-style (border-top-style, border-right-style,
      border-bottom-style, border-left-style)
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
        <div class="example-brick border-style-double">
          <div class="example-brick-small"></div>
        </div>
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
</template>

<script>
export default {
  name: "BordersView",
};
</script>

<style scoped lang="scss">
* {
  box-sizing: border-box;
}

.example-group {
  & > :not(:last-child) {
    margin-bottom: 0.5rem;
  }

  .example-brick {
    background-color: lightblue;
    width: 8rem;
    height: 4rem;
    margin-right: 1rem;
    border-width: 0.75rem;

    .example-brick-small {
      width: 4rem;
      height: 2rem;
    }
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
