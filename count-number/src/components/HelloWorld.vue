<template>
  <div>
    <div class="hello">
      <h1>{{ counter }}</h1>
    </div>
    <div>
      <button @click="plusNum">+</button>&nbsp;&nbsp;
      <button @click="minusNum">-</button>
    </div>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  data() {
    return {
      counter: 0,
    };
  },
  methods: {
    plusNum() {
      this.counter++;
    },
    minusNum() {
       this.counter--;
    },
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
