<template>
  <div class="positive">
     <h1>Positive Card</h1>
     <div v-if="history.length > 0"> 
      <h2>{{ lastReceived }} </h2>
     </div>
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
  name: 'positive',
  data () {
    return {
      lastReceived: 3,
      history: [4, 2, 1, 3]
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
