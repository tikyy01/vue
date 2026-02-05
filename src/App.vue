<script>
export default {
  name: 'App',
  data() {
    return {
      visible: true
    }
  },
  methods: {
    toggle: function() {
      this.visible = !this.visible;
    }
  }
}
</script>

<template>
  <button @click="toggle">
    {{ visible ? 'Скрыть абзац' : 'Показать абзац' }}
  </button>
  <p v-show="visible">Тогглируемый абзац</p>
</template>