<template>
  <div class="education">
    <spinner />
    <b-row class="mx-2 text-left">
      <b-col cols="sm-12" class="mt-0 mb-2">
        <b-card id="card-education">
          <b-card-text id="card-text">
            <b-icon size="sm" class=" mb-0 mr-3" icon="archive" aria-hidden="true"></b-icon>Education</b-card-text>
            <hr>
            <b-tabs id="containertabs" small>
            <b-tab title="College" active>
                  <b-jumbotron class="text-center hoverable">
                    <b-row>
                       <b-col md="4" offsetMd="1" class="m-3">
                          <b-img fluid :src="require('../assets/photo/slsu.png')" width="250px"></b-img>
                          <p id="year">2015-2019</p>
                       </b-col>
                       <b-col md="7" class="text-md-left ml-1 mt-3">
                          <p id="schoolname" class="pt-auto mb-0">Southern Leyte State University - Main Campus</p>
                          <p id="address">Sogod, Southern Leyte</p>
                          <p id="course" class="mt-3 mb-0">Bachelor of Science in Information Technology <span id="major">Major in Networking</span></p>
                          <br><span id="address">Website:  </span>
                          <a href="http://slsuonline.edu.ph/index.php/en/" target="_blank" id="schoolink">www.slsuonline.edu.ph</a>
                       </b-col>
                    </b-row>
                   </b-jumbotron>
            </b-tab>
             <b-tab title="High School" active>
                  <b-jumbotron class="text-center hoverable">
                    <b-row>
                       <b-col md="4" offsetMd="1" class="m-3">
                          <b-img fluid :src="require('../assets/photo/dafenhs.png')" width="250px"></b-img>
                          <p id="year">2010-2014</p>
                       </b-col>
                       <b-col md="7" class="text-md-left ml-1 mt-3">
                          <p id="schoolname" class="pt-auto mb-0">Don Agustin F. Escaño National High School</p>
                          <p id="address">Bogo, Tomas Oppus, Southern Leyte</p>
                           <p id="course" class="mt-3 mb-0">High School Student</p>
                          <br><span id="address">Website:  </span>
                           <a href="http://www.facebook.com/dafenhs.page.shs.jhs/" target="_blank" id="schoolink">www.facebook.com/dafenhs.page</a>
                       </b-col>
                    </b-row>
                   </b-jumbotron>
            </b-tab>
             <b-tab title="Elementary" active>
                  <b-jumbotron class="text-center hoverable">
                    <b-row>
                       <b-col md="4" offsetMd="1" class="m-3">
                          <b-img fluid :src="require('../assets/photo/Tocslogo.png')" width="250px"></b-img>
                          <p id="year">2003-2009</p>
                       </b-col>
                       <b-col md="7" class="text-md-left ml-1 mt-3">
                          <p id="schoolname" class="pt-auto mb-0">Tomas Oppus Central School</p>
                          <p id="address">Bogo, Tomas Oppus, Southern Leyte</p>
                          <p id="course" class="mt-3 mb-0">Elementary Student</p>
                          <br><span id="address">Website:  </span>
                          <a href="https://www.facebook.com/tomasoppus.central" target="_blank" id="schoolink">  www.facebook.com/tomasoppus.central</a>
                       </b-col>
                    </b-row>
                   </b-jumbotron>
            </b-tab>
            </b-tabs>
        </b-card>
      </b-col>
    </b-row>
  </div>
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Hammersmith+One&family=Oleo+Script&family=Squada+One&family=Teko&display=swap');
  .education{
    margin-top: 20px;
  }
   #card-education{
    background: #212121;
  }
  #card-text{
    font-size: 15px;
    font-weight: bolder;
    color: #fff;
  }

  .nav-tabs .nav-item.show .nav-link, .nav-tabs .nav-link.active{
    background: #394988;
    color: #fff;
    border: none;
    transition: all 0.5s;
  }
  .nav-tabs .nav-item.show .nav-link, .nav-tabs .nav-link:hover{
    background: #394988;
    border: none;
    transition: all 0.5s;
  }
  a{
    color: #fff;
  }
  
  a:hover{
    color: #A8B3DB;
  }
  #schoolname { 
    font-family: 'Squada One';
    font-size: 35px;
    font-weight: bolder;
    color: #3a4d91;
}
#address{
    font-family: 'Teko';
    font-size: 20px;
    font-weight: lighter;
    color: #3a4d91;
}
 #course{
    font-family: 'Hammersmith One';
    font-size: 20px;
    font-weight: bolder;
    color: #3a4d91;
  }
  #major{
    font-family: 'Hammersmith One';
    font-size: 20px;
    font-weight: lighter;
    color: #64DD17;
  }
  #year{
      font-family: 'Oleo Script';
      font-size: 27px;
      font-weight: bolder;
      color: #64DD17;
  }
  #schoolink{
      font-family: 'Oleo Script';
      font-size: 25px;
      color: #64DD17;
  }
</style>