<script setup>
import { reactive, ref } from "vue";

const count = ref(1);

const increase = () => {
  count.value++;
};

const submitForm = (e) => {
  // e.preventDefault();
  console.log(`Form submitted with count: ${count.value}`);
};
</script>

<template>
  <form @submit.prevent="submitForm">
    <div>{{ count }}</div>
    <!-- <button v-on:click="increase">Increase</button> -->
    <button @click="increase" type="button">Increase</button>
    <button type="submit">Submit</button>
  </form>
</template>

<style>
.red {
  color: red;
}
</style>
