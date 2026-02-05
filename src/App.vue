<script>
export default {
  name: 'App',
  data() {
    return {
      age: 25
    }
  }
}
</script>

<template>
  <p v-if="age < 18">подросток</p>
  <p v-else-if="age >= 19 && age <= 25">молодой человек</p>
  <p v-else-if="age >= 26">мужчина</p>
</template>