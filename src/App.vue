<template>
  <div id="app">
    <div id="nav">
      <Navbar />
      <vue-page-transition name="fade-in-right" class="content">

      <router-view />  <!-- DYNAMIC CONTENT LOADED -->

    </vue-page-transition>
    </div>
    <router-view />
        <Footer />
  </div>
</template>
<script>
export default {
  components: {
    Navbar: () => import('@/components/Navbar'),
    Footer: () => import('@/components/Footer'),
  }
}
</script>

<style lang="scss">

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

   hr{
  background: #ffff;
}

#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #ffffff;
    }
  }
}
.bg{
   /* The image used */
    background-color: #2c3e50;
}
</style>
