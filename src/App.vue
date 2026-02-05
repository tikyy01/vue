<script>
export default {
  name: 'App',
  data() {
    return {
      arr: ['x', 'y', 'z']
    }
  }
}
</script>

<template>
  <ul>
    <li v-for="(elem, key) in arr" :key="key">
      {{ key + 1 }}
    </li>
  </ul>
</template>