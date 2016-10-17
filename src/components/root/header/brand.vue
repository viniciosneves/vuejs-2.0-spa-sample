<script>
export default {

  name: 'confee-header-brand',

  methods: {
    toggle () {
      this.$emit('toggle')
    }
  }

}
</script>

<template>

  <div class="navbar-header">
      <button type="button" class="navbar-toggle" data-toggle="collapse" data-target="#bs-example-navbar-collapse-1" @click="toggle">
          <span class="sr-only">Toggle navigation</span>
          <span class="icon-bar"></span>
          <span class="icon-bar"></span>
          <span class="icon-bar"></span>
      </button>
      <router-link class="navbar-brand" to="/">Confee</router-link>
  </div>

</template>
