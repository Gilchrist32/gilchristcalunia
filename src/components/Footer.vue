<template>
    <div>
      <footer class="bd-footer text-muted docs-border">
        <b-row class="justify-content-center container">
          <b-container class="text-left">
              <b-row class="mt-1">
                  <b-col  md="3" lg="3" xl="3" class="mx-auto mt-1">
                     <b-img fluid :src="require('../assets/photo/logogc1.png')" width="250px"></b-img>
                     <p class="name">GC Website & Portfolio</p>
                     <span class="name">
                      I'm a Web Developer and Freelance Designer based Philippines. I create innovative solutions that make your product or
                      service more effective in the marketplace.
                    </span>
                  </b-col>
              <b-col md="4" lg="4" xl="4" class="mx-auto mt-1">
                <h5 class="ttitle">| CONTACT INFO</h5>
                <ul class="ul-contactus">
                  <li><b-icon icon="envelope" /> calunia32@gmail.com</li>
                  <li><b-icon icon="phone" />Call Me: 09365657801 / 09334371899</li>
                  <li>
                    <b-icon icon="geo-alt" /> Tomas Oppus, Southern Leyte, Philippines
                  </li>
                </ul>
              </b-col>
              <b-col md="4" lg="4" xl="4" class="mx-auto mt-1">
                <h5 class="ttitle">| STAY CONNECTED & FOLLOW</h5>
                <span class="name">
                    Subscribe to our WT Emai Mailing List and Please Follow us on our Social Media Profile in order to keep updated.
                </span>
                <b-input-group class="mt-3">
                    <b-form-input placeholder="Email Address"></b-form-input>
                    <b-button id="subs" variant="info">Subscribe</b-button>
                </b-input-group>
                <br>
                  <b-avatar href="https://www.facebook.com/gilchrist.calunia" target="_blank" id="facebooklink" v-b-tooltip.hover title="Add or Follow me on Facebook"><font-awesome-icon :icon="['fab', 'facebook']" /></b-avatar>&nbsp;
                  <b-avatar href="https://www.instagram.com/gilchristcalunia" target="_blank" id="instagramlink" v-b-tooltip.hover title="Add or Follow me on Instagram"><font-awesome-icon :icon="['fab', 'fa-instagram']" /></b-avatar>&nbsp;
                  <b-avatar href="https://github.com/Gilchrist32" target="_blank" id="githublink" v-b-tooltip.hover title="Follow me on Github and give a star for my repositories"><font-awesome-icon :icon="['fab', 'github']" /></b-avatar>&nbsp;
              </b-col>
            </b-row>
          </b-container>
        </b-row>
      </footer>
      <div class="footer-copyright">
        <b-container>
              <b-row class="d-flex align-items-center">
              <b-col md="8" lg="8">
               <p class="text-left">Created By: GC Personal Web Developed | &copy; {{ new Date().getFullYear() }}  All Right Reserved</p>
              </b-col>
              </b-row>
        </b-container>
        </div>
  </div>
</template>

<style lang="scss" scoped>
footer {
  background: #0e152c;
  margin-top: 10px;
  padding: 60px 0;
  display: flex;
  justify-content: center;
  align-items: center;
}
.ologo{
  border-radius: 3px;
  margin-top: -20px;
}
.name {
  color: #fff;
  font-size: 13px;
  font-size: 13px;
}
.ul-contactus li {
  list-style-type: none !important;
  color: #eeeeee;
  font-size: 15px;
}
ul li {
  list-style-type: none;
  position: relative;
  right: 40px;
  color: #eeeeee;
  font-size: 12px;
}
ul li a {
  color: #eeeeee;
}
ul li a:hover {
  color: #fff;
}
.ttitle {
  font-family: 'Teko';
  color: #388E3C;
  font-size: 30px;
}
#subs{
  background-color: #D50000;
}
.footer-copyright {
  text-align: center;
  font-size: 12px;
  color: #fff;
  padding: 10px 0;
  background: #080d1d;
  cursor: default;
}
</style>