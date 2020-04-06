<template>
  <h1>Perfil do usuário: {{ $route.params.id }}</h1>
</template>

<script>
export default {
  validate(data) {
    const id = data.params.id
    return /^\d+$/.test(id)
  },
  layout: 'users'
}
</script>
