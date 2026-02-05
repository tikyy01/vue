<script>
export default {
  name: 'App',
  data() {
    return {
      visible: true
    }
  }
}
</script>

<template>
  <p v-if="visible">Первый абзац (виден при visible=true)</p>
  <p v-else>Второй абзац (виден при visible=false)</p>
</template>