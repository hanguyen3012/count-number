<template>
  <div>
    <div class="hello">
      <h1>{{counter}}</h1>
    </div>
    <div>
      <button v-on:click="counter +=1">+</button>&nbsp;&nbsp;
      <button v-on:click="counter -=1">-</button>
    </div>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  data (){
    return {
      counter : 0,
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
