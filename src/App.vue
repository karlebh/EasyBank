<template>
  <div id="app">
    <Header/>

    <MobileMain/>
    <DesktopMain/>

    <Footer/>
  </div>
</template>

<script>
  import Header from '@/components/Header'
  import Footer from '@/components/Footer'
  import MobileMain from '@/components/MobileMain'
  import DesktopMain from '@/components/DesktopMain'

  export default {
    name: 'App',
    data() {
      return {}
    },
    components: {
      Header,
      MobileMain,
      DesktopMain,
      Footer,
    },
  }
</script>

<style>
  #app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }
</style>
