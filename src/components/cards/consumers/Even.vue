<template>
  <div class="even">
     <h1>Even Card</h1>
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
  name: 'even',
  data () {
    return {
      lastReceived: 2,
      history: [4, 2]
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
