// Copied HTML and CSS from: https://codepen.io/gkioultsin/pen/pcbHI
<template>
<div class="calculator">
	<input class="calculator__screen" v-model="result"/>
	<div class="calculator__keyboard">
    <button class="key key--red"     value="">C</button>
    <button class="key key--default" value="-">⬅</button>
    <button class="key key--default" value="-+">±</button>
    <button class="key key--blue"    value="/">÷</button>
    <button class="key key--default" value="7">7</button>
    <button class="key key--default" value="8">8</button>
    <button class="key key--default" value="9">9</button>
    <button class="key key--blue"    value="*">×</button>
    <button class="key key--default" value="4">4</button>
    <button class="key key--default" value="5">5</button>
    <button class="key key--default" value="6">6</button>
    <button class="key key--blue"    value="-">-</button>
    <button class="key key--default" value="1">1</button>
    <button class="key key--default" value="2">2</button>
    <button class="key key--default" value="3">3</button>
    <button class="key key--blue"    value="+">+</button>
    <button class="key key--default" value="0">0</button>
    <button class="key key--default" value=".">.</button>
    <button class="key key--double"  value="=">=</button>
  </div>
</div>
</template>

<script>
export default {
  name: 'Calculator',
  data: function () {
    return {
      result: '0'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
@charset "utf-8";

.calculator {
	width:240px;
	height:auto;
	margin:3% auto;
	background:#ccc;
	border-radius:20px;
	-moz-box-shadow:inset 0 0 12px #FFF,
	inset 0px 1px #E6E6E6, 0 1px 1px #323643,
	inset 0px 1px #7b839b, 0 2px 5px rgba(0,0,0,.5);
	-webkit-box-shadow:inset 0 0 12px #FFF,
	inset 0px 1px #E6E6E6, 0 1px 1px #323643,
	inset 0px 1px #7b839b, 0 2px 5px rgba(0,0,0,.5);
	box-shadow:inset 0 0 12px #FFF,
	inset 0px 1px #E6E6E6, 0 1px 1px #323643,
	inset 0px 1px #7b839b, 0 2px 5px rgba(0,0,0,.5);
}
.calculator__screen{
	width:86%;
	height:54px;
	margin:20px 0px 0px 12px;
	padding-right:9px;
	background:#858585;
	text-align:right;
	border-radius:6px;
	border:1px solid #6B6B6B;
	font-size:26px;
	font:"Trebuchet MS", Arial, Helvetica, sans-serif;
	-moz-box-shadow:inset 0 0 10px #333,
	inset 0 1px 1px #0A0B0D, 0px 1px #E6E6E6;
	-webkit-box-shadow:inset 0 0 10px #333,
	inset 0 1px 1px #0A0B0D, 0px 1px #E6E6E6;
	box-shadow:inset 0 0 10px #333,
	inset 0 1px 1px #0A0B0D, 0px 1px #E6E6E6;
}
.calculator__screen:focus{
	outline:none;
}
.calculator__keyboard {
	width:220px;
	margin:12px;
}
.key {
  color: #CCC;
	width:45px;
	height:45px;
	padding:0;
	margin:0px 0px 10px 5px;
	border-radius:6px;
  font:24px "Trebuchet MS", Arial, Helvetica, sans-serif;
	line-height: 45px;
}
.key--default {
  border:1px solid #333;
	-moz-box-shadow:inset 0 0 10px #666,
	inset 0px 1px #BCD6FF, 0 1px 1px #323643;
	-webkit-box-shadow:inset 0 0 10px #666,
	inset 0px 1px #BCD6FF, 0 1px 1px #323643;
	box-shadow:inset 0 0 10px #666,
	inset 0px 1px #BCD6FF, 0 1px 1px #323643;
	background:#333;
}
.key:active {
	color:#FFF;
	border:1px solid #333;
	-moz-box-shadow:inset 0 1px 1px #0A0B0D, 0px 1px #E6E6E6;
	-webkit-box-shadow:inset 0 1px 1px #000, 0px 1px #E6E6E6;
	box-shadow:inset 0 1px 1px #000, 0px 1px #E6E6E6;
}
.key:focus{
  outline: none;
}
.key--red {
	background-color:#d02200;
	border:1px solid #d02200;
	-moz-box-shadow:inset 0 0 10px #F63,
	inset 0px 1px #BCD6FF, 0 1px 1px #323643;
	-webkit-box-shadow:inset 0 0 10px #F63,
	inset 0px 1px #BCD6FF, 0 1px 1px #323643;
	box-shadow:inset 0 0 10px #F63,
	inset 0px 1px #BCD6FF, 0 1px 1px #323643;
}
.key--double {
	width:100px;
	background-color: #036;
	border:1px solid #036;
	-moz-box-shadow:inset 0 0 10px #069,
	inset 0px 1px #BCD6FF, 0 1px 1px #323643;
	-webkit-box-shadow:inset 0 0 10px #069,
	inset 0px 1px #BCD6FF, 0 1px 1px #323643;
	box-shadow:inset 0 0 10px #069,
	inset 0px 1px #BCD6FF, 0 1px 1px #323643;
}
.key--double:active {
	border:1px solid #039;
	-moz-box-shadow:inset 0 1px 1px #0A0B0D, 0px 1px #E6E6E6;
	-webkit-box-shadow:inset 0 1px 1px #0A0B0D, 0px 1px #E6E6E6;
	box-shadow:inset 0 1px 1px #0A0B0D, 0px 1px #E6E6E6;
}
.key--blue {
	background-color: #036;
	border:1px solid #036;
	-moz-box-shadow:inset 0 0 10px #069,
	inset 0px 1px #BCD6FF, 0 1px 1px #323643;
	-webkit-box-shadow:inset 0 0 10px #069,
	inset 0px 1px #BCD6FF, 0 1px 1px #323643;
	box-shadow:inset 0 0 10px #069,
	inset 0px 1px #BCD6FF, 0 1px 1px #323643;
}
.key--blue:active {
	border:1px solid transparent;
	-moz-box-shadow:inset 0 1px 1px #0A0B0D, 0px 1px #E6E6E6;
	-webkit-box-shadow:inset 0 1px 1px #0A0B0D, 0px 1px #E6E6E6;
	box-shadow:inset 0 1px 1px #0A0B0D, 0px 1px #E6E6E6;
}

</style>