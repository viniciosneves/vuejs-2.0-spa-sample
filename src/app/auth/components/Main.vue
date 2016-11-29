<script>
import Login from './forms/Login'
import { mapGetters } from 'vuex'
export default {
  components: { Login },
  name: 'Auth',
  computed: {
    ...mapGetters(['isLogged'])
  }
}
</script>

<template>

  <div>
    <header class="page-header row">

      <h2>Vue 2.0 - Auth</h2>

    </header>

    <Login></Login>
  </div>

</template>
