<script>
export default {
  name: 'App',
  data() {
    return {
      isAdmin: true
    }
  }
}
</script>

<template>
  <p v-if="isAdmin">Администратор</p>
  <p v-else>Пользователь</p>
</template>