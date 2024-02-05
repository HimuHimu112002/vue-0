<script setup>
import { ref } from 'vue'
import { reactive } from 'vue'
const count = ref(10)
const state = reactive({ count: 0 })
</script>
<template>
  <h1>This is Welcome components</h1>
  <button @click="count = count + 10">Count is: {{ count }}</button> <br/>
  <button @click="state.count++">{{ state.count }}</button><br/>
</template>
