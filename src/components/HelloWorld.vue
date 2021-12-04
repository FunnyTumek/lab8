<template>
  <div>
    <h1>Fibonacci</h1>
    <div>
      <label for="nr">K = </label>
      <input id="nr" type="number" v-model="k" min="1" max="400"/>
    </div>
    <div>
      Fibonacci({{k}}) =  {{ wynik }}
    </div>
  </div>
</template>

<script>
export default {
  name: "Fibonacci",
  data: function () {
    return { k: 1 };
  },
  methods: {
    calculateFibo: function (result, counter) {
      if (counter === 0) {
        return 0;
      } else if (counter === 1) {
        return 1;
      } else {
        return (
          this.calculateFibo(result, counter - 2) +
          this.calculateFibo(result, counter - 1)
        );
      }
    },
  },
  computed: {
    wynik: function () {
      return this.calculateFibo(0, this.k);
    },
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
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
