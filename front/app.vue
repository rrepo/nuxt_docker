<template>
  <div>
    <p>test</p>
  </div>
</template>

<script setup lang="ts">
const {data} = await useFetch('https://jsonplaceholder.typicode.com/posts/');

console.log(data.value)

const test = await useFetch('https://jsonplaceholder.typicode.com/posts/');

console.log(test)
console.log(test.data.value)

const go = await useFetch('http://localhost:8080/albums');
console.log(go.data.value)

</script>
