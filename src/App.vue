<template>
  <div>
    <h1>{{ title }}</h1>
    <h1>{{ count }}</h1>
    <button @click="onClickCount">Click</button>
    <button @click="onClickClear">Clear</button>
  </div>
</template>

<script>
export default {
  name: "app",
  data() {
    return {
      title: "Test-VueJs",
      count: 0,
    };
  },
  methods: {
    onClickCount() {
      this.count = this.count + 1;
    },
    onClickClear() {
      this.count = 0;
    },
  },
};
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
</style>
