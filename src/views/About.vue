<template>
  <div class="about">
    <spinner />
    <b-row class="mx-2 text-left">
      <b-col cols="sm-8" class="mt-0 mb-2">
        <b-card id="card-about">
          <b-card-text id="card-text">
            <b-icon size="sm" class=" mb-0 mr-3" icon="person-fill" aria-hidden="true"></b-icon>About Me</b-card-text>
            <hr>
            <b-row>
              <b-col cols="sm-6">
                <b-form-group class="label" label="First Name">
                  <b-form-input class="text-input" value="Gilchrist" disabled></b-form-input>
                </b-form-group>
              </b-col>
               <b-col cols="sm-6">
                <b-form-group class="label" label="Last Name">
                  <b-form-input class="text-input" value="Calunia" disabled></b-form-input>
                </b-form-group>
              </b-col>
               <b-col cols="sm-6">
                <b-form-group class="label" label="Middle Name">
                  <b-form-input class="text-input" value="Abrea" disabled></b-form-input>
                </b-form-group>
              </b-col>
              <b-col cols="sm-6">
                <b-form-group class="label" label="Age">
                  <b-form-input class="text-input" value="22" disabled></b-form-input>
                </b-form-group>
              </b-col>
              <b-col cols="sm-6">
                <b-form-group class="label" label="Birth Date">
                  <b-form-input class="text-input" value="September 04, 1997" disabled></b-form-input>
                </b-form-group>
              </b-col>
              <b-col cols="sm-6">
                <b-form-group class="label" label="Civil Status">
                  <b-form-input class="text-input" value="Single" disabled></b-form-input>
                </b-form-group>
              </b-col>
              <b-col cols="sm-6">
                <b-form-group class="label" label="Gender">
                  <b-form-input class="text-input" value="Male" disabled></b-form-input>
                </b-form-group>
              </b-col>
              <b-col cols="sm-6">
                <b-form-group class="label" label="Religious">
                  <b-form-input class="text-input" value="Roman Catholic"></b-form-input>
                </b-form-group>
              </b-col>
               <b-col cols="sm-6">
                <b-form-group class="label" label="Address">
                  <b-form-input class="text-input" value="San Agustin, Tomas Oppus, Southern Leyte"></b-form-input>
                </b-form-group>
              </b-col>
              <b-col cols="sm-6">
                <b-form-group class="label" label="Gmail">
                  <b-form-input class="text-input" value="calunia32@gmail.com"></b-form-input>
                </b-form-group>
              </b-col>
              <b-col cols="sm-12 mb-6">
                  <b-form-group class="label" label="Bio">
                     <b-form-textarea class="text-input" rows="6" value="Responsible for designing, coding and modifying websites, from layout to function and according to a client's specifications. Strive to create visually appealing sites that feature user-friendly design and clear navigation."></b-form-textarea>
                  </b-form-group>
              </b-col>
            </b-row>
        </b-card>
      </b-col>
      <Infocard />
    </b-row>
    <Workex />
  </div>
</template>
<script>
export default {
  components: {
    Spinner: () => import('@/components/Spinner'),
    Infocard: () => import('@/components/Infocard'),
    Workex: () => import('@/components/Workex')
  }
}
</script>

<style>
  .about{
    margin-top: 20px;
  }
  #card-about{
    background: #212121;
    color: #3a4d91;
  }
  #card-text{
    font-size: 15px;
    font-weight: bolder;
    color: #fff;
  }
  .label{
    font-size: 13px;
    color: #BDBDBD;
    font-weight: bolder;
  }
  .text-input{
    background: #424242 !important;
    border: 0 !important;
    color: #C0CA33 !important;
    font-size: 14px;
  }
  #position{
    color: #C0CA33;
    font-size: 20px;
  }
  #details{
    font-size: 13px;
  }
  #facebooklink{
    background: #3f67b3;
  }
  #instagramlink{
    background: #FF1744;
  }
  #githublink{
    background: #545B62;
  }
  #address{
    font-size: 15px;
    color: #fff;
  }
</style>
