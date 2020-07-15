<template>
 <b-col cols="sm-4"  class="mt-0 mb-auto">
        <b-card id="card-about" no-body class="overflow-hidden mb-2" style="max-width: 540px;">
          <b-row no-gutters>
              <b-card-img :src="require('@/assets/photo/gilchrist.png')" alt="Center image"  class="pl-4"></b-card-img>
                <b-card-body id="card-text" class="text-center" title="Gilchrist Calunia">
                    <b-card-text id="position">Web Developer</b-card-text>
                  <b-card-text id="details">
                  Contact Details:<br>
                  TM - 093365657801 / SUN - 09334371899
                  </b-card-text>
                  <b-avatar href="https://www.facebook.com/gilchrist.calunia" target="_blank" id="facebooklink" v-b-tooltip.hover title="Add or Follow me on Facebook"><font-awesome-icon :icon="['fab', 'facebook']" /></b-avatar>&nbsp;
                  <b-avatar href="https://www.instagram.com/gilchristcalunia" target="_blank" id="instagramlink" v-b-tooltip.hover title="Add or Follow me on Instagram"><font-awesome-icon :icon="['fa', 'instagram']" /></b-avatar>&nbsp;
                  <b-avatar href="https://github.com/Gilchrist32" target="_blank" id="githublink" v-b-tooltip.hover title="Follow me on Github and give a star for my repositories"><font-awesome-icon :icon="['fab', 'github']" /></b-avatar>&nbsp;
              </b-card-body>

          </b-row>
        </b-card>
      </b-col>
 </template>
 

        
