<template>
  <div>
    <button @click="testing">Test</button>
  </div>
</template>


<script setup>

const testing = () => {
  const { data, error } = useFetch('./api/hello')
  console.log("data",data.value)
  console.log("error", error.value)
}

</script>