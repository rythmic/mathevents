<template>
  <div id="app">
    <div class="cardSpace">
      
      <div class="card">
        <all></all>
      </div>

      <div class="card">
        <addition></addition>
      </div>
      <div class="card">
        <subtraction></subtraction>
      </div>
      <div class="card">
        <multiplication></multiplication>
      </div>
      <div class="card">
        <division></division>
      </div>
      
      <div class="card">
        <even></even>
      </div>
      <div class="card">
        <odd></odd>
      </div>

      <div class="card">
        <positive></positive>
      </div>
      <div class="card">
        <negative></negative>
      </div>
    </div>
  </div>
</template>

<script>
import Addition from './components/cards/consumers/Addition'
import Subtraction from './components/cards/consumers/Subtraction'
import Multiplication from './components/cards/consumers/Multiplication'
import Division from './components/cards/consumers/Division'
import Even from './components/cards/consumers/Even'
import Odd from './components/cards/consumers/Odd'
import Positive from './components/cards/consumers/Positive'
import Negative from './components/cards/consumers/Negative'
import All from './components/cards/consumers/All'

export default {
  name: 'app',
  components: {
    Addition,
    Subtraction,
    Multiplication,
    Division,
    Even,
    Odd,
    Positive,
    Negative,
    All
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
  margin-top: 30px;
}
.cardSpace {
  display: flex;
  padding: 10px;
  border: 1px #aaa solid;
  width: 900px;
  flex-wrap: nowrap;
  flex-direction: row;
  margin: 0 auto;
}

.card {
  border: 2px #000 solid;
  padding: 10px;
}

</style>
