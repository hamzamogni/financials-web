<template>
    <p>{{ message }}</p>
</template>
<script setup>
import { inject } from "vue";

const message = inject("message");
</script>