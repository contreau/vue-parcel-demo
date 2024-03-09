<script setup>
import { ref } from "vue";
import Message from "./Message.vue";
const count = ref(0);
const date = ref({ month: "March", day: 9, year: 2024 });
</script>

<template>
  <Message></Message>
  <button @click="count++">You've clicked me {{ count }} time(s).</button>
  <p>It is {{ date.month }} {{ date.day }}, {{ date.year }}</p>
</template>

<style>
body {
  background-color: #233040;
  color: #ffffff;
  font-family: system-ui;
  text-align: center;
}
</style>
