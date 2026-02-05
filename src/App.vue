<script>
export default {
  name: 'App',
  data() {
    return {
      items: [1, 2, 3, 4, 5]
    }
  }
}
</script>

<template>
  <!-- Задание 1: Каждый элемент в своем div -->
  <div v-for="item in items" :key="item">{{ item }}</div>
  
  <!-- Задание 2: Квадрат каждого элемента -->
  <div v-for="item in items" :key="'sq' + item">{{ item * item }}</div>
  
  <!-- Задание 3: Элементы в виде списка ul -->
  <ul>
    <li v-for="item in items" :key="item">{{ item }}</li>
  </ul>
</template>