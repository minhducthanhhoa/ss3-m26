<template>
  <div>
    Bài 5
    <button v-on:click="handleClick">Click me</button>
  </div>
</template>

<script setup>
    const handleClick = ()=>{
        console.log("Clicked");
        
    }
</script>

<style>

</style>