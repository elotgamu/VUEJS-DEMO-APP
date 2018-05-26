<template lang="html">
  <div class="page signin">

    <div class="container">
      <div class="row">
        <!-- <div class="col-sm-12 text-center">
          <h1>{{ msg }}</h1>
        </div> -->

        <div class="col-sm-12 col-lg-6 offset-lg-3">

          <div class="card mb-3">
            <div class="card-header">
              <h1>{{ msg }}</h1>
            </div>

            <div class="card-body">
              <div class="signin-form form-group">
                <input class="form-control mb-3" v-model="email" placeholder="Email">
                <input class="form-control mb-3" type="password" v-model="password" placeholder="Password">
              </div>
            </div>

            <div class="card-footer">
              <div class="">
                <input type="button" class="btn btn-default" v-on:click="reset" value="Reset">
                <input type="submit" class="btn btn-primary" v-on:click="login" value="Login">
              </div>
            </div>

          </div>

        </div>

        <div class="col-sm-12 text-center">
          <router-link to="/">Go back to Home</router-link>
        </div>
      </div>
    </div>

  </div>
</template>

<script>
export default {
  name: 'signin',
  data () {
    return {
      msg: 'Signin page',
      email: '',
      password: ''
    }
  },
  methods: {
    login () {
      console.log(this.email)
      console.log(this.password)
    },
    reset () {
      this.email = ''
      this.password = ''
    }
  }
}
</script>

<style lang="scss" scoped>
// .signin {
//   width: 550px;
//   margin: 0 auto;
//   .signin-form {
//     // margin: 0 120px;
//     div {
//       margin: 6px 0;
//     }
//   }
// }
//
// h1, h2 {
//   font-weight: normal;
// }
//
// ul {
//   list-style-type: none;
//   padding: 0;
//   li {
//     display: inline-block;
//     margin: 10px 10px;
//     padding: 3px 10px;
//   }
// }
//
// a {
//   color: #42b983;
// }
//
// .language-panel {
//   margin: 5px 0 20px;
//   .language-btn {
//     cursor: pointer;
//   }
// }
</style>
