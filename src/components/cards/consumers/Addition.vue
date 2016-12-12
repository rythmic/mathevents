<template>
  <div class="addition">
     <h1>Addition Card</h1> 
     <h2>{{ firstNumber }} + {{ secondNumber }} = {{ firstNumber + secondNumber}}  </h2>

     <div>
      <h4>History</h4>
        <ul>
        <li>Last Received: {{ lastReceived }}</li>
        <li> History: {{ history }}</li>
     </div>
 </div>
</template>

<script>
export default {
  name: 'addition',
  data () {
    return {
      firstNumber: 1,
      secondNumber: 3,
      lastReceived: 3,
      history: [-5, -3, 4, 2, 1, 3]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

a {
  color: #42b983;
}
</style>
