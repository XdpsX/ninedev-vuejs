<script setup>
import { reactive, ref } from "vue";

// ref su dung 1 doi tuong va 1 thuoc tinh
// truy cap thuoc tinh ref: .value
// const count = ref(0);
// count.value = count.value + 1;

// su dung 1 object trong do co nhieu doi tuong
// truy cap thuoc tinh ko can .value
const count2 = reactive(ref([]));
const count = reactive({
  title: "VueJS s",
  author: "Top",
});
</script>

<template>
  <div class="red">This is {{ count.title }}</div>
</template>

<style>
.red {
  color: red;
}
</style>
