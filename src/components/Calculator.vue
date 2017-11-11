// Copied HTML and CSS from: https://codepen.io/gkioultsin/pen/pcbHI
<template>
<div class="calculator">
	<input id="screen" class="screen" v-model="result"/>
	<div class="buttons">
    <button id="clear" value="">C</button>
    <button id="backspace" value="-">⬅</button>
    <button id="sign" value="-+">±</button>
    <button id="divide" value="/">÷</button>
    <button class="digit" value="7">7</button>
    <button class="digit" value="8">8</button>
    <button class="digit" value="9">9</button>
    <button id="multiply" value="*">×</button>
    <button class="digit" value="4">4</button>
    <button class="digit" value="5">5</button>
    <button class="digit" value="6">6</button>
    <button id="minus" value="-">-</button>
    <button class="digit" value="1">1</button>
    <button class="digit" value="2">2</button>
    <button class="digit" value="3">3</button>
    <button id="plus" value="+">+</button>
    <button class="digit" value="0">0</button>
    <button class="digit" value=".">.</button>
    <button id="equal" value="=">=</button>
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

.calculator{
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
.screen{
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
.screen:focus{
	outline:none;
}
.buttons{
	width:220px;
	margin:12px;
}
.buttons button{
	width:45px;
	height:45px;
	padding:0;
	margin:0px 0px 10px 5px;
	border:1px solid #333;
	border-radius:6px;
	color:#CCC;
	font:24px "Trebuchet MS", Arial, Helvetica, sans-serif;
	line-height: 45px;
	-moz-box-shadow:inset 0 0 10px #666,
	inset 0px 1px #BCD6FF, 0 1px 1px #323643;
	-webkit-box-shadow:inset 0 0 10px #666,
	inset 0px 1px #BCD6FF, 0 1px 1px #323643;
	box-shadow:inset 0 0 10px #666,
	inset 0px 1px #BCD6FF, 0 1px 1px #323643;
	background:#333;
}
.buttons button:active {
	color:#FFF;
	border:1px solid #333;
	-moz-box-shadow:inset 0 1px 1px #0A0B0D, 0px 1px #E6E6E6;
	-webkit-box-shadow:inset 0 1px 1px #000, 0px 1px #E6E6E6;
	box-shadow:inset 0 1px 1px #000, 0px 1px #E6E6E6;
}
#clear{
	background-color:#d02200;
	border:1px solid #d02200;
	-moz-box-shadow:inset 0 0 10px #F63,
	inset 0px 1px #BCD6FF, 0 1px 1px #323643;
	-webkit-box-shadow:inset 0 0 10px #F63,
	inset 0px 1px #BCD6FF, 0 1px 1px #323643;
	box-shadow:inset 0 0 10px #F63,
	inset 0px 1px #BCD6FF, 0 1px 1px #323643;

}
#clear:active{
	border:1px solid #d02200;
	-moz-box-shadow:inset 0 1px 1px #0A0B0D, 0px 1px #E6E6E6;
	-webkit-box-shadow:inset 0 1px 1px #0A0B0D, 0px 1px #E6E6E6;
	box-shadow:inset 0 1px 1px #0A0B0D, 0px 1px #E6E6E6;
}
#equal{
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
#equal:active{
	border:1px solid #039;
	-moz-box-shadow:inset 0 1px 1px #0A0B0D, 0px 1px #E6E6E6;
	-webkit-box-shadow:inset 0 1px 1px #0A0B0D, 0px 1px #E6E6E6;
	box-shadow:inset 0 1px 1px #0A0B0D, 0px 1px #E6E6E6;
}
#minus, #plus, #divide, #multiply{
	background-color: #036;
	border:1px solid #036;
	-moz-box-shadow:inset 0 0 10px #069,
	inset 0px 1px #BCD6FF, 0 1px 1px #323643;
	-webkit-box-shadow:inset 0 0 10px #069,
	inset 0px 1px #BCD6FF, 0 1px 1px #323643;
	box-shadow:inset 0 0 10px #069,
	inset 0px 1px #BCD6FF, 0 1px 1px #323643;
}
#minus:active, #plus:active, #divide:active, #multiply:active{
	border:1px solid transparent;
	-moz-box-shadow:inset 0 1px 1px #0A0B0D, 0px 1px #E6E6E6;
	-webkit-box-shadow:inset 0 1px 1px #0A0B0D, 0px 1px #E6E6E6;
	box-shadow:inset 0 1px 1px #0A0B0D, 0px 1px #E6E6E6;
}

</style>