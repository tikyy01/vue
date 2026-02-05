<script>
export default {
  name: 'App',
  data() {
    return {
      obj: {
        user1: '100$',
        user2: '200$',
        user3: '300$'
      }
    }
  }
}
</script>

<template>
  <!-- Задание 1 -->
  <ul>
    <li v-for="value in obj" :key="value">{{ value }}</li>
  </ul>
  
  <!-- Задание 2 -->
  <ul>
    <li v-for="(value, key) in obj" :key="key">{{ key }} - {{ value }}</li>
  </ul>
  
  <!-- Задание 3 -->
  <ul>
    <li v-for="(value, key, index) in obj" :key="key">{{ key }} - {{ value }} - {{ index }}</li>
  </ul>
  
  <!-- Задание 4 -->
  <ul>
    <li v-for="(value, key, index) in obj" :key="key">{{ key }} - {{ value }} - {{ index + 1 }}</li>
  </ul>
</template>