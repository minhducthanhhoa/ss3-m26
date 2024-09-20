<template>
  <div>
    Bài 6
    <button v-on:click="handlegetParam('Rikkei Academy')">Get param</button>
  </div>
</template>

<script setup>
    const handlegetParam = (name)=>{
        console.log("name", name);
        
    }
</script>

<style>

</style>