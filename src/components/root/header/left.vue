<script>
export default {
  name: 'confee-header-left'
}
</script>

<template>

  <!-- Collect the nav links, forms, and other content for toggling -->
    <ul class="nav navbar-nav">

        <router-link :to="{name: 'dashboard.main'}" tag="li">
            <a>Home</a>
        </router-link>

        <router-link to="/auth" tag="li">
            <a>Auth</a>
        </router-link>

    </ul>
  <!-- /.navbar-collapse -->

</template>
