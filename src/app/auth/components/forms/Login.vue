<template lang="html">
    <div class="row">
      <div class="col-md-6">
        <div class="form-group">
          <label>E-mail</label>
          <input type="email" name="email" v-model="user.email" value="" class="form-control">
        </div>
        <div class="form-group">
          <label>Password</label>
            <input type="password" v-model="user.password" class="form-control">
        </div>
        <button class="btn btn-primary" :disabled="!isValid" @click="doLogin">Sign In</button>
      </div>
    </div>
</template>

<script>
import { isEmpty } from 'lodash'
export default {
  data () {
    return {
      user: {
        email: '',
        passwaord: ''
      }
    }
  },
  computed: {
    isValid () {
      const user = this.user
      return !isEmpty(user.email) && !isEmpty(user.password)
    }
  },
  mounted () {},
  methods: {
    doLogin () {
      this.$router.push('/')
    }
  },
  components: {}
}
</script>

<style lang="css">
</style>
