<template>
  <div>
    <button v-on:click="handleClick">Click me</button>
    <button v-on:click="handleDelete(1)">Delete</button>
    <button @click="handleGetEvent">Event Info</button>
    <form @submit.prevent="handleSubmit">
        <button type="submit"></button>
    </form>
    <button @keydown.esc="handleCloseForm">Đóng form</button>
  </div>
</template>

<script setup>
    const handleClick = ()=> {
        console.log("Clicked");
    }
    const handleDelete = (id)=>{
        console.log("id", id);
        
    }
    const handleGetEvent = (event)=>{
        console.log("event", event);
        
    }
    const handleSubmit = ()=>{
        alert("submited");
    }
    const handleCloseForm =()=>{
        alert("Đóng form");
    }
</script>

<style>

</style>