<script setup lang="ts">
import { ref } from "vue";

const testCount = ref(0);

function handleClick() {
  console.log(testCount.value);
  testCount.value = testCount.value + 1;
}
</script>

<template>
  <button
    style="
      border: 0 solid #e2e8f0;
      margin-top: 10px;
      background-color: rgb(246, 179, 82);
      border-radius: 0.25rem;
      font-weight: 700;
      padding: 0.5rem 1rem 0.5rem 1rem;
      color: rgb(24, 24, 24);
    "
    @click="handleClick"
  >
    Remote counter: {{ testCount }}
  </button>
</template>

<style scoped />
