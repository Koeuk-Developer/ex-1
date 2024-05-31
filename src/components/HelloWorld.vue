<template>
  <div class="hello">
    <div class="container"  >
      <h1>{{number}}</h1>
      <button v-on:click="increment(count)" class="btn btn-info mt-3 ">Increment++</button>
      <br>
      <button v-on:click="decrement(count)" class="btn btn-info">Decrement--</button>
      <br>
      <input type="number" v-model="count">
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      number: 0,
      count: 0,
    }
  },
  methods: {
    increment(c) {
      return this.number += c;
    },
    decrement(c) {
      return this.number -= c;
    },
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.container {
  margin: 10px;
}

h3 {
  margin: 40px 0 0;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}

</style>
