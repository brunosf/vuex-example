<template>
  <div class="">
    <div id="app">{{ count }}</div>
    <button @click="increment">+1</button>
    <button @click="decrement">-1</button>
  </div>
</template>

<script>
export default {
  name: "app",
  computed: {
    count() {
      return this.$store.state.count;
    }
  },
  methods: {
    increment() {
      return this.$store.commit("increment");
    },
    decrement() {
      return this.$store.commit("decrement");
    }
  }
};
</script>

<style></style>
