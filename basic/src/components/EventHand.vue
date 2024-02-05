<script setup>
    function say(message) {
    alert(message)
    }
</script>

<template>
    <h1>Event handling components</h1>
    <button @click="say('hello')">Say hello</button>
    <button @click="say('bye')">Say bye</button>
</template>