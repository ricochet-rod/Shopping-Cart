<template>
<div>
  <h1>{{ name }}</h1>
  <button class="btn" @click="placeOrder">Place you order!</button>
</div>
</template>

<script>
export default {
  setup() {
    const name = "The Snazzy Burger";
    console.log(name);
    const placeOrder = () => alert("Your order has been placed!");
    return {
      name,
      placeOrder
    };
  },
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

</style>
