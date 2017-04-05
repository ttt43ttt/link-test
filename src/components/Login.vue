<template>
  <div class="login">
    <h3>Login to TestLink</h3>
    <div class="container">
      <div class="form-group row">
        <label for="username" class="col-sm-2 col-form-label">Username:</label>
        <div class="col-sm-10">
          <input id="username" type="text" class="form-control" placeholder="Username" v-model="username"/>
        </div>
      </div>
      <div class="form-group row">
        <label for="password" class="col-sm-2 col-form-label">Password:</label>
        <div class="col-sm-10">
          <input id="password" type="password" class="form-control" placeholder="Password" v-model="password"/>
        </div>
      </div>
      <div class="form-group">
        <input type="button" class="btn btn-primary" value="Submit" v-on:click="login"/>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'login',
    data () {
      return {
        username: '',
        password: '',
        error: 'Your username or password is incorrect'
      }
    },
    methods: {
      login: function () {
        console.log(`username is ${this.username}`);
        console.log(`password is ${this.password}`);
      }
    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
