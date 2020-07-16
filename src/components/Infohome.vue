<template>
  <div class="bg">
    <b-infohome>
      <b-mask class="gradient d-flex justify-content-center align-items-center">
          <b-container>
              <b-row>
                  <div class="white-text text-center text-md-left col-md-6 mt-xl-5 mb-6 mt-3  ">
                    <h6 id="twel" class="h6-responsive font-weight-bold mt-sm-3">Wellcome! I'm</h6>
                    <h1 id="mname" class="h6-responsive font-weight-bold">GILCHRIST CALUNIA</h1>
                    <h6 id="quo" class="mb-4 font-weight-bold">Information Technology, Front-end Web Developer.</h6>
                      <hr class="my-4"> 
                       <b-button variant="success" pill id="btngithub" href="https://github.com/Gilchrist32/gilchristcalunia-portfolio" target="_blank" size="md">
                    <b-icon size="sm" class="ml-1 mt-0 mr-2" icon="inbox-fill" variant="warning"></b-icon>
                    <span id="chat">LET'S CHAT</span></b-button>&nbsp;
                    <b-button variant="outline-success" pill id="btngithub" href="https://github.com/Gilchrist32/gilchristcalunia-portfolio" target="_blank" size="md">
                    <b-icon size="sm" class="ml-1 mt-0 mr-2" icon="arrow-down-circle-fill" variant="success"></b-icon>
                    <span id="chat">ABOUT ME</span></b-button>ABOUT
                  </div>
                   <b-col md="6" xl="5" class="mt-xl-5 ml-8">
                      <b-img :src="require('@/assets/photo/profile.png')" alt="image fluid" width="340px"></b-img>
            </b-col>
              </b-row>
          </b-container>
    </b-mask> 
    </b-infohome>
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
@import url('https://fonts.googleapis.com/css2?family=Kaushan+Script&family=Righteous&family=Lobster&family=Balsamiq+Sans&display=swap');
.bg{
    background: url('../assets/photo/background.jpg') center ;
}
 #twel{
    font-family: 'Kaushan Script';
    font-size: 23px;
    color: #ffffff;
    padding-top: 25px;
  }
#mname{
    font-family: 'Righteous';
    color: #3F51B5;
    font-size: 50px;
  }
#quo{
    font-family: 'Lobster';
    font-size: 23px;
    font-weight: bolder;
    color: #ffffff;
    }
#chat{
  color: #ffffff;
  font-family: 'Balsamiq Sans';
}
</style>