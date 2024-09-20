<template>
  <div>
    <img v-bind:src="url" alt="">
    <button v-bind:disabled="isdisabled">Click me</button>
    <input type="text" v-bind:disabled="isdisabled">
    <div v-bind="divAtribute">container</div>
    <p v-bind="attribute">Nội dung</p>
    <div v-bind:class="{textRed: isTextRed}">hello world</div>
  </div>
  
</template>

<script setup>
  const url = "https://images2.thanhnien.vn/528068263637045248/2024/1/25/e093e9cfc9027d6a142358d24d2ee350-65a11ac2af785880-17061562929701875684912.jpg";
  const isdisabled = true;
  const divAtribute = {
    id:"container-id",
    class:"container-class",
  }
  const attribute = {
    id:"paragraph",
    area:"paragraph"
  }
  const isTextRed = true
</script>

<style>
  .textRed{
    color: red;
  }
</style>