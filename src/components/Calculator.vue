<template>
  <h1>CursedLator</h1>
  <div class="calc">
    <div class="display">Enter a number</div>

    <div class="keypad">
      <div class="num1">1</div>
      <div class="num2">2</div>
      <div class="num3">3</div>
      <div class="plusKey">+</div>

      <div class="num4">4</div>
      <div class="num5">5</div>
      <div class="num6">6</div>
      <div class="minusKey">-</div>

      <div class="num7">7</div>
      <div class="num8">8</div>
      <div class="num9">9</div>
      <div class="multiplyKey">x</div>

      <div class="ac key">AC</div>
      <div class="num0">0</div>
      <div class="divideKey">/</div>
      <div class="equalKey">=</div>
    </div>
  </div>
</template>

<style>
.calc {
  width: 320px;
  height: 480px;
  display: flex;
  flex-direction: column;
  margin-left: auto;
  margin-right: auto;
  background-color: #d9d3c7;
  border: 2px solid #d9d3c7;
}

.display {
  flex: 1;
  background-color: #a5b3a6;
  margin: 10px;
  font-size: 40px;
  text-align: right;
  overflow-wrap: break-word;
  padding: 5px;
}

.keypad {
  height: 320px;
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 8px;
  margin: 10px;
}

.key {
  display: flex;
  justify-content: center;
  align-items: center;
  font-size: 40px;
  cursor: pointer;
}
.num {
  background-color: #525759;
  color: #ffffff;
}
.fn {
  background-color: #877569;
  color: #000000;
}
.special {
  background-color: #bd5a04;
  color: #000000;
  font-size: 35px;
  font-weight: bold;
}
::selection {
  background: none;
}
</style>
