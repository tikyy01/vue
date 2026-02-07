<script>
export default {
  name: 'App',
  data() {
    return {
      items: [1, -2, 3, -4, 5]
    }
  }
}
</script>

<template>
  <ul>
    <template v-for="item in items">
      <li v-if="item > 0" :key="item">{{ item }}</li>
    </template>
  </ul>
</template>