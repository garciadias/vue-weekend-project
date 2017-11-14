<template>
  <div id="app">
    <Calculator></Calculator>
  </div>
</template>

<script>
import Calculator from './components/Calculator'

export default {
  name: 'app',
  components: {
    Calculator
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
body {
	background-image: -moz-radial-gradient(center, circle closest-corner, #353863 0%, #000 100%);
	background-image: -o-radial-gradient(center, circle closest-corner, #353863 0%, #000 100%);
	background-image: -webkit-radial-gradient(center, circle closest-corner, #353863 0%, #000 100%);
	-webkit-user-select:none;
	-moz-user-select:none;
	-ms-user-select:none;
	-o-user-select:none;
	user-select:none;
}
</style>
