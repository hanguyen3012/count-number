<template>
  <div>
    <div>
      Enter your number: <input v-model="value" @focusout="handleOutFocus()" />
    </div>
    <div class="hello">
      <h1>{{ counter }}</h1>
    </div>
    <div>
      <button class="btn1" @click="plusNum">+</button>
      <button class="btn2" @click="minusNum">-</button>
    </div>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  data: () => ({
    counter: 0,
    value: 1,
  }),
  methods: {
    handleOutFocus() {
      if (!this.value) {
        this.value = 1;
      }
    },
    plusNum() {
      this.counter = this.counter + this.value;
      return this.counter;
    },
    minusNum() {
      this.counter = this.counter - this.value;
      return this.counter;
    },
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.btn2 {
  margin-left: 50px;
}
</style>
