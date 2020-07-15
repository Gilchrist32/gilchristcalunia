<template>
    <div class="fixed-top top">
        <b-navbar toggleable="lg" id="navigationbar" type="dark">
            <b-navbar-brand route to="/" class="ml-2">
                <b-img fluid :src="require('../assets/photo/logogc1.png')" width="250px"></b-img>
            </b-navbar-brand>
            <b-navbar-toggle target="collapse" @click="toggle = !toggle">
                <b-icon v-if="expanded" icon="chevron-bar-up"></b-icon>
            </b-navbar-toggle>
            
            <b-collapse v-model="toggle" is-nav>
                <b-navbar-nav class="ml-auto mr-5">
                     <router-link to="/" :class="$route.path == '/' ? 'nav-link active' : 'nav-link'" id="tag">
                     <b-icon size="sm" class="ml-3 mb-2 mr-3" icon="house-door" aria-hidden="true"></b-icon>HOME</router-link>
                     <router-link to="/about" :class="$route.path == '/about' ? 'nav-link active' : 'nav-link'" id="tag">
                     <b-icon size="sm" class="ml-3 mb-2 mr-3" icon="person-fill" aria-hidden="true"></b-icon>ABOUT</router-link>
                     <router-link to="/education" :class="$route.path == '/education' ? 'nav-link active' : 'nav-link'" id="tag">
                     <b-icon size="sm" class="ml-3 mb-2 mr-3" icon="archive" aria-hidden="true"></b-icon>EDUCATION</router-link>
                     <router-link to="/project" :class="$route.path == '/project' ? 'nav-link active' : 'nav-link'" id="tag">
                     <b-icon size="sm" class="ml-3 mb-2 mr-3" icon="file-earmark-text" aria-hidden="true"></b-icon>PROJECT</router-link>
                </b-navbar-nav>
            </b-collapse>
        </b-navbar>
    </div>     
</template>
<script>
export default {
     data: () => ({
    toggle: false
  })
}
</script>
<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Teko&display=swap');

 #navigationbar{
    background: #0E152C;
    padding: 5px;
    box-shadow: 1px 1px #1D2B5A;

  }
  #tag{
      font-family: 'Teko';
      font-size: 20px;
      color: #0277BD;
  }


</style>
