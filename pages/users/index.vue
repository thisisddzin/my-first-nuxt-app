<template>
  <div class="container">
    <input v-model="userId" type="text" />
    <button @click="onLoadUser">Ir para usuário selecionado</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      userId: ''
    }
  },

  methods: {
    onLoadUser() {
      this.$router.push('/users/' + this.userId)
    },
    layout: 'users'
  }
}
</script>
