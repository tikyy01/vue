<script>
export default {
  name: 'App',
  data() {
    return {
      items: ['a', 'b', 'c', 'd', 'e']
    }
  },
  methods: {
    addItem: function() {
      this.items.push('новый');
    },
    removeFirst: function() {
      this.items.shift();
    },
    removeLast: function() {
      this.items.pop();
    },
    removeSecondLast: function() {
      if (this.items.length >= 2) {
        this.items.splice(this.items.length - 2, 1);
      }
    },
    sortItems: function() {
      this.items.sort();
    },
    reverseItems: function() {
      this.items.reverse();
    }
  }
}
</script>

<template>
  <ul>
    <li v-for="item in items" :key="item">{{ item }}</li>
  </ul>
  <button @click="addItem">Добавить в конец</button>
  <button @click="removeFirst">Удалить первый</button>
  <button @click="removeLast">Удалить последний</button>
  <button @click="removeSecondLast">Удалить предпоследний</button>
  <button @click="sortItems">Сортировать</button>
  <button @click="reverseItems">Обратный порядок</button>
</template>