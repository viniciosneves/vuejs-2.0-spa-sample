<script>
import Left from './left'
import Brand from './brand'

export default {

  name: 'confee-header',

  components: { Left, Brand },

  data () {
    return { isOpen: false }
  },

  methods: {

    onToggleMenu () {
      this.isOpen = !this.isOpen
    }
  }
}

</script>

<template>

  <!-- Navigation -->
  <nav class="navbar navbar-inverse navbar-fixed-top" role="navigation">
      <div class="container">
          <!-- Brand and toggle get grouped for better mobile display -->

            <Brand @toggle="onToggleMenu"></Brand>

          <!-- Collect the nav links, forms, and other content for toggling -->
          <div class="collapse navbar-collapse" :class="{ in: isOpen }">

            <Left></Left>

          </div>
          <!-- /.navbar-collapse -->
      </div>
      <!-- /.container -->
  </nav>

</template>
