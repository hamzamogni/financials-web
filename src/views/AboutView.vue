<template>
  <div class="about">
    <TestA />
  </div>
</template>
<script setup>
import { onMounted, provide, ref } from "vue";
import TestA from "@/components/TestA.vue";

const msg = ref(1);

onMounted(() => {
  msg.value++;
});

provide("message", msg);
</script>

<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style>
