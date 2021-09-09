<template>
  <img alt="Vue logo" src="./assets/logo.png" :ref="(el) => (someref = el)" />
  <HelloWorld msg="Hello Vue 3 + TypeScript + Vite" />
</template>

<script lang="ts" setup>
import { Ref, ref } from 'vue';
import HelloWorld from './components/HelloWorld.vue';

const someref: Ref<HTMLElement | null> = ref(null);
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
