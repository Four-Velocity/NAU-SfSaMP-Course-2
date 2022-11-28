<template>
  <div id="t4-main">
    <div class="result">0</div>
    <div class="buttons">
      <v-btn class="operator" id="rst">AC</v-btn>
      <v-btn class="operator secondary" id="pm" variant="tonal">±</v-btn>
      <v-btn class="operator secondary" id="percent" variant="tonal">%</v-btn>
      <v-btn class="operator" id="div">÷</v-btn>
      <v-btn class="digit" id="seven" variant="outlined">7</v-btn>
      <v-btn class="digit" id="eight" variant="outlined">8</v-btn>
      <v-btn class="digit" id="nine" variant="outlined">9</v-btn>
      <v-btn class="operator" id="mult">✕</v-btn>
      <v-btn class="digit" id="four" variant="outlined">4</v-btn>
      <v-btn class="digit" id="five" variant="outlined">5</v-btn>
      <v-btn class="digit" id="six" variant="outlined">6</v-btn>
      <v-btn class="operator" id="minus">-</v-btn>
      <v-btn class="digit" id="one" variant="outlined">7</v-btn>
      <v-btn class="digit" id="two" variant="outlined">8</v-btn>
      <v-btn class="digit" id="three" variant="outlined">9</v-btn>
      <v-btn class="operator" id="plus">+</v-btn>
      <v-btn class="digit" id="zero" variant="outlined">0</v-btn>
      <v-btn class="operator secondary" id="dot" variant="tonal">.</v-btn>
      <v-btn class="operator" id="equal">=</v-btn>
    </div>
  </div>
</template>

<style scoped>
#t4-main {
  flex: 0 1 60%;
  min-width: 90vw;
  display: flex;
  flex-wrap: wrap;
  gap: 5px;
}
.buttons,
.result {
  display: flex;
  flex: 0 1 100%;
  flex-wrap: wrap;
  justify-content: flex-start;
}

.buttons {
  /* gap: 5px; */
  justify-content: center;
}

.result {
  height: 50px;
  border-radius: 15px;
  background: black;
  color: white;
  font-size: 1.5em;
  justify-content: flex-end;
  align-items: center;
  padding: 0 25px;
}

button {
  display: flex;
  flex: 0 1 25%;
  justify-content: center;
  align-items: center;
  height: 50px;
  font-size: 2em;
}

#zero {
  flex-grow: 2;
}

.secondary {
  border: 1px solid;
}
</style>