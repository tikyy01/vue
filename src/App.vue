<script>
export default {
  name: 'App',
  data() {
    return {
      clicked: false
    }
  },
  methods: {
    // Задание 1: Ссылка без перехода
    handleLinkClick: function(event) {
      event.preventDefault();
      alert('Переход по ссылке предотвращен');
    },
    
    // Задание 2: Однократный клик по кнопке
    handleButtonClick: function() {
      if (!this.clicked) {
        alert('Первый и последний клик!');
        this.clicked = true;
      }
    }
  }
}
</script>

<template>
  <!-- Задание 1 -->
  <a href="https://example.com" @click="handleLinkClick">
    Ссылка (клик без перехода)
  </a>
  
  <br><br>
  
  <!-- Задание 2 -->
  <button @click="handleButtonClick">
    Кнопка (только первый клик)
  </button>
</template>