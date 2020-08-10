<template>
  <div>
    <navigation />
    <div class="content">
      <Nuxt />
    </div>
  </div>
</template>

<script>
import Navigation from '@/components/Navigation'
export default {
  component: { Navigation }
}
</script>

<style>
* {
  box-sizing: border-box;
  color: whitesmoke
}

body {
  background: #2d3536;
  color: whitesmoke;
  font-family: Arial, Helvetica, sans-serif;
  margin: 0;
}

.content {
  padding: 2rem;
}
</style>
