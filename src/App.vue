<script>
export default {
  name: 'App',
  data() {
    return {
      hidden: true
    }
  }
}
</script>

<template>
  <p v-if="!hidden">text</p>
</template>