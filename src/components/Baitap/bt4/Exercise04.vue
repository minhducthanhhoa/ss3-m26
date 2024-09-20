<template>
  <div>
    Bài 4
    <p v-bind:class="{textBlue: isTextBlue}">Block</p>
  </div>
</template>

<script setup>
    const isTextBlue = true;
</script>

<style scoped>
    .textBlue{
        color: white;
        background-color: blue;
    }
</style>