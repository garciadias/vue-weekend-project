<template>
  <div class="digit-canvas">
    <div class="screen">
      <div class="output">
        0
      </div>
    </div>
    <div class='key_row'>
      <button class='key'>7</button>
      <button class='key'>8</button>
      <button class='key'>9</button>
      <button class='key'>&nbsp;-</button>
    </div>     
    <div class='key_row'>
      <button class='key'>4</button>
      <button class='key'>5</button>
      <button class='key'>6</button>
      <button class='key'>+</button>
    </div>     
    <div class='key_row'>
      <button class='key'>1</button>
      <button class='key'>2</button>
      <button class='key'>3</button>
      <button class='key'>=</button>
    </div>     
  </div>
</template>

<script>
export default {
  name: 'Calculator',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.digit-canvas {
  background-color: black;
  border: 1px solid orange;
  width: 40%;
  height: 700px;
  display: inline-flex;
  flex-direction: column;
}

.key {
  font-size: 2.0em;
  color: black;
  background-color: orange;
  flex-grow: 1;
}

.key_row {
  display: flex;
  justify-content: center;
  flex-grow: 1;
}

.screen {
  /* width: 100%; */
  font-size: 6.0em;
  background: grey;
  flex-grow: 1;
  display: flex;
  justify-content: flex-end;
  align-items: stretch;
}

.output {
  align-self: flex-end;
  }
</style>