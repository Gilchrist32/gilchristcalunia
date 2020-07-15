<template>
  <div class="bg">
    <b-infohome>
      <b-row class="justify-content-center text-center">
        <b-col cols="sm-12">
          
          <h1 class="mt-2 mb-1" id="j-1">Jerome Villaruel</h1>
          <h4 class="mb-2" id="j-2">
            Information Technology, Web Developer and UX & UI Designer.
          </h4>
          <b-avatar href="https://facebook.com/veoscript" target="_blank" id="facebooklink" v-b-tooltip.hover title="Add or Follow me on Facebook"><font-awesome-icon :icon="['fab', 'facebook']" /></b-avatar>&nbsp;
          <b-avatar href="https://twitter.com/VeoScript43" target="_blank" id="twitterlink" v-b-tooltip.hover title="Follow me on Twitter"><font-awesome-icon :icon="['fab', 'twitter']" /></b-avatar>&nbsp;
          <b-avatar href="https://github.com/VeoScript" target="_blank" id="githublink" v-b-tooltip.hover title="Follow me on Github and give a star for my repositories"><font-awesome-icon :icon="['fab', 'github']" /></b-avatar>&nbsp;
           
          <hr class="my-4">
        </b-col>

        <b-col cols="sm-12">
          <p class="text-center">
            Subscribe and Follow me to all of my social media accounts for more info and projects.
          </p>
        </b-col>
      </b-row>
    </b-infohome>
    <b-container>
    </b-container>
  </div>
</template>

<script>

export default {
  name: 'Infohome',
  components: {


  }
}
</script>

<style>
.bg{
    background: url('../assets/photo/background.jpg') center ;
}
  .jumbotron{
    background: #24315E;
    border-radius: 0px;
    color: #A8D1E7;
    margin-top: 75px;
  }
  #n-subscribers{
    color: #ECAB44;
  }
  #j-1{
    font-family: 'Monoton';
    font-size: 35px;
    color: #DEACF5;
  }
  #j-2{
    font-family: 'Varela Round';
    font-size: 20px;
    font-weight: bolder;
    color: #fff;
  }
  #facebooklink{
    background: #3f67b3;
  }
  #twitterlink{
    background: #1EACFF;
  }
  #githublink{
    background: #545B62;
  }
</style>