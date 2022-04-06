<template>
  <div>
    <div>Enter your number: <input type ="number" v-model= "valueInput"/></div>
    <div class="hello">
      <h1>{{ counter + valueInput }}</h1>
    </div>
    <div>
      <button class = "btn1" @click="plusNum">+</button>
      <button class = "btn2" @click="minusNum">-</button>
    </div>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  data() {
    return {
      valueInput: 1,
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
.btn2{
  margin-left: 50px;
}
</style>
