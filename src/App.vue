<script>
export default {
  name: 'App',
  data() {
    return {
      cost: 100,
      amount: 3
    }
  },
  computed: {
    price: function() {
      return this.cost * this.amount;
    }
  },
  methods: {
    changeCost: function() {
      this.cost = 150;
    }
  }
}
</script>

<template>
  <div>
    <!-- Вывод данных -->
    <p>Цена: {{ cost }}</p>
    <p>Количество: {{ amount }}</p>
    <p>Общая стоимость: {{ price }}</p>
    
    <!-- Кнопка для изменения стоимости -->
    <button @click="changeCost">Изменить цену на 150</button>
  </div>
</template>