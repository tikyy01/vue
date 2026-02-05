<script>
export default {
  name: 'App',
  data() {
    return {
      items: [1, 2, 3]
    }
  }
}
</script>

<template>
  <!-- Задание 1 -->
  <div v-for="item in items" :key="item">
    <p>{{ item }}</p>
    <p class="divider"></p>
  </div>
  
  <!-- Задание 2 -->
  <ul>
    <template v-for="item in items">
      <li :key="item">{{ item }}</li>
      <li class="divider" :key="'div' + item"></li>
    </template>
  </ul>
</template>