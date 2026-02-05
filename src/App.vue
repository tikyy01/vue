<script>
export default {
  name: 'App',
  data() {
    return {
      visible: false
    }
  },
  methods: {
    show: function() {
      this.visible = true;
    },
    hide: function() {
      this.visible = false;
    }
  }
}
</script>

<template>
  <!-- Задание 1: Кнопка для показа абзаца -->
  <button @click="show">Показать абзац</button>
  <p v-if="visible">Этот абзац можно показывать и скрывать</p>
  
  <!-- Задание 2: Две кнопки для показа и скрытия -->
  <div style="margin-top: 20px;">
    <button @click="show">Показать</button>
    <button @click="hide">Скрыть</button>
    <p v-if="visible">Абзац с двумя кнопками управления</p>
  </div>
  
  <!-- Задание 3: Только одна видимая кнопка -->
  <div style="margin-top: 20px;">
    <button v-if="!visible" @click="show">Показать абзац</button>
    <button v-else @click="hide">Скрыть абзац</button>
    <p v-if="visible">Абзац с умной кнопкой</p>
  </div>
</template>