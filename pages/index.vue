<template>
  <h1>My first Nuxt APP 😁</h1>
</template>

<script>
export default {
  head () {
    return {
      title: 'Nuxt App! | Home',
      meta: [
        {
          name: 'description',
          content: 'Website about posts'
        }
      ],
      htmlAttrs: {
        lang: 'en'
      }
    }
  }
}
</script>
