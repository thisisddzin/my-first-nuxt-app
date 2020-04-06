<template>
  <div class="container">
    <h1>
      {{
        $route.params.id != null ? '' : 'Olá digite um usuário para pesquisar'
      }}
    </h1>
    <nuxt-child />
  </div>
</template>

<script>
export default {
  layout: 'users'
}
</script>
