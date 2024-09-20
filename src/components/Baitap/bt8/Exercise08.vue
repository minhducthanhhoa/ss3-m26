<template>
  <div>
    <a href="http://www.google.com" @click.prevent="checkLink">Click vào liên kết</a>
    <p v-if="errorMessage" style="color: red;">{{ errorMessage }}</p>
  </div>
</template>

<script setup>
import { ref } from 'vue'

const errorMessage = ref('')

const checkLink = (event) => {
  const url = event.target.href

  if (!url.startsWith('https://')) {
    event.preventDefault()

    errorMessage.value = 'Đường dẫn không hợp lệ.'
  } else {
    errorMessage.value = ''
  }
}
</script>

<style scoped>

a {
  color: blue;
  text-decoration: underline;
  cursor: pointer;
}
</style>
