<script setup>
defineProps({
  name: {
    type: String,
  },
})
</script>

<template>
  <h2>Hey your first component {{ name }}</h2>
</template>
