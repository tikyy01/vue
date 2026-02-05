<script>
export default {
  name: 'App',
  data() {
    return {
      day: 3, // Текущий день недели
      days: ['Воскресенье', 'Понедельник', 'Вторник', 'Среда', 'Четверг', 'Пятница', 'Суббота']
    }
  }
}
</script>

<template>
  <p v-for="(dayName, index) in days" :key="index" v-if="day === index">
    {{ dayName }}
  </p>
</template>