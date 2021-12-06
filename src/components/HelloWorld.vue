<script setup>
import { ref } from "vue";
import { Button } from "ant-design-vue";

defineProps({
  msg: String,
});

const count = ref(0);
</script>

<template>
  <h1>{{ msg }}</h1>

  <Button @click="count++">+</Button>
  {{ count }}
  <Button @click="count--">-</Button>
</template>

<style scoped></style>
