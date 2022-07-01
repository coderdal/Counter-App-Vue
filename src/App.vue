<template>
  <h2>My first Vue JS project</h2>
  <h1>Counter App</h1>

  <h1 class="count">{{ count }}</h1>

  <button @click="count++">+</button>
  <button @click="count--" class="down">-</button>
</template>

<script>
// eslint-disable-next-line

export default {
  name: "App",
  data() {
    return {
      count: 0,
    };
  },
};
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

.count {
  color: #3a85cf;
}

button {
  width: 80px;
  height: 30px;
  font-size: 20px;
  font-weight: 600;
  background: #3b9b3b;
  color: #fff;
  border-radius: 5px;
  border: none;
  cursor: pointer;
  margin: 0 5px;
}

.down {
  background: #fc4040;
}
</style>
