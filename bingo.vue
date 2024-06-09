<script setup>
import { ref } from 'vue'
import { reactive } from 'vue'

const counter = reactive({
  count: 0
})

console.log(counter.count) // 0
counter.count++

const message = ref('Hello World!')
console.log(message.value) // "Hello World!"
message.value = 'Changed'
// component logic
// declare some reactive state here.
</script>

<template>
  <h1>{{ message }}</h1>
  <h1>{{ message.split('').reverse().join('') }}</h1>
  <p>Count is: {{ counter.count }}</p>
</template>