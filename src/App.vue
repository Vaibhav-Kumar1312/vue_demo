<template>
  <img
    alt="Vue logo"
    src="./assets/logo.png"
  >
  <HelloWorld :msg="message" />
</template>

<script lang="ts">
import { defineComponent } from "vue";
import HelloWorld from "./components/HelloWorld.vue";

export default defineComponent({
  name: "App",
  components: {
    HelloWorld,
  },
  data: () => ({
    message: "Welcome to Your Vue.js + TypeScript App",
  }),
  methods: {
    printHello(count: number) {
      for (let i = 0; i < count; i += 1) {
        console.log("Hello there");
      }
    },
  },
});
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
