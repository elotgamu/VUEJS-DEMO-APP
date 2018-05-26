<template>
  <div id="app">

    <!-- <loading :loadingStatus="loadingStatus"></loading> -->
    <img src="./assets/logo.png">
    <router-view></router-view>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld'
// import Loading from './components/notices/Loading'

export default {
  name: 'App',
  // components: {
  //   'loading': Loading,
  //
  // },
  data: () => ({
    loadingStatus: '',
    alertStatus: {},
    intervalId: ''
  }),
  created () {
    // do something after creating vue instance
    // this.$bus.$on('isLoading', (event) => {
    //   this.loadingStatus = event
    // })
  }
}
</script>

<style>
#app {
  /* font-family: 'Avenir', Helvetica, Arial, sans-serif; */
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
