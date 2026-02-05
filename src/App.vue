<script>
export default {
  name: 'App',
  data() {
    return {
      visible1: true,
      visible2: true,
      visible3: true
    }
  },
  methods: {
    toggle1: function() {
      this.visible1 = !this.visible1;
    },
    toggle2: function() {
      this.visible2 = !this.visible2;
    },
    toggle3: function() {
      this.visible3 = !this.visible3;
    }
  }
}
</script>

<template>
  <button @click="toggle1">Тогглить абзац 1</button>
  <p v-if="visible1">Абзац 1</p>
  
  <button @click="toggle2">Тогглить абзац 2</button>
  <p v-if="visible2">Абзац 2</p>
  
  <button @click="toggle3">Тогглить абзац 3</button>
  <p v-if="visible3">Абзац 3</p>
</template>