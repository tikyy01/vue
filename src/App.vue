<script>
export default {
  name: 'App',
  data() {
    return {
      showParagraphs: true
    }
  },
  methods: {
    toggleParagraphs: function() {
      this.showParagraphs = !this.showParagraphs;
    }
  }
}
</script>

<template>
  <button @click="toggleParagraphs">
    {{ showParagraphs ? 'Скрыть абзацы' : 'Показать абзацы' }}
  </button>
  
  <template v-if="showParagraphs">
    <p>Первый абзац</p>
    <p>Второй абзац</p>
    <p>Третий абзац</p>
  </template>
</template>