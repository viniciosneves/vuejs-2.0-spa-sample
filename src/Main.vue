<template>
  <header class="page-header row">
    <h2>Vue 2.0</h2>
    <h3 v-show="$route.params.name">Seja bem vindo, {{ $route.params.name }}</h3>
  </header>
</template>

<script>
    export default {

    }
</script>
