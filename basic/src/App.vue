<script setup>
import HelloWorld from './components/HelloWorld.vue'
import TheWelcome from './components/TheWelcome.vue'
import WelcomeItem from './components/WelcomeItem.vue';
import { reactive } from 'vue'
import { ref } from 'vue'
const count = ref(10)
const state = reactive({ count: 0 })

</script>

<template>
  <header>
    <h1>Aktarujjaman</h1>
  </header>

  <main>
    <WelcomeItem/>
    <HelloWorld/>
    <TheWelcome/>
    <button @click="count = count + 10">Count is: {{ count }}</button> <br/>

    <button @click="state.count++">{{ state.count }}</button>
  </main>
</template>

<style scoped>

</style>
