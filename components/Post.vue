<template>
  <div>
    <p>{{ id }}. {{ title }}</p>
  </div>
</template>

<script>
export default {
  name: 'Post',
  props: {
    id: { type: String, default: '', required: true },
    title: { type: String, default: '', required: true }
  }
}
</script>
