<template>
  <div class="main">
    <div class="header">
      <div class="container">
        <nav class="navbar navbar-expand-lg bg-faded fixed-top" style="background-color: #727F80;border-bottom: 2px solid #007BFF;" :class="{showBar: scrollPosition < 20, hideBar: scrollPosition > 20}">
          <a class="navbar-brand" href="#">SUKANTA BALA</a>
          <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarTogglerDemo01" aria-controls="navbarTogglerDemo01" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon">
              <i class="fa fa-bars" aria-hidden="true"></i>
            </span>
          </button>
          <div class="collapse navbar-collapse navbar-item" id="navbarTogglerDemo01">
            <ul class="navbar-nav ml-auto">
              <li class="nav-item">
                <a class="nav-link" v-scroll-to="'#about'">ABOUT ME</a>
              </li>
              <li class="nav-item">
                <a class="nav-link" v-scroll-to="'#services'">SERVICES</a>
              </li>
              <li class="nav-item">
                <a class="nav-link" v-scroll-to="'#portfolio'">PORTFOLIO</a>
              </li>
              <li class="nav-item">
                <a class="nav-link" v-scroll-to="'#team'">OUR TEAM</a>
              </li>
              <li class="nav-item">
                <a class="nav-link" v-scroll-to="'#feedback'">FEEDBACK</a>
              </li>
              <li class="nav-item">
                <a class="nav-link" v-scroll-to="'#contact'">CONTACT ME</a>
              </li>
            </ul>
          </div>
        </nav>
      </div>
    </div>
  </div>
</template>

<script>
import Vue from 'vue'
import vueScrollto from 'vue-scrollto'
Vue.use(vueScrollto)
export default {
  data () {
    return {
      scrollPosition: null
    }
  },

  methods: {
    updateScroll () {
      this.scrollPosition = window.scrollY
    }
  },

  mounted () {
    window.addEventListener('scroll', this.updateScroll)
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

  .showBar {
  height: 80px;
  -webkit-transition: all 0.3s ease-out;
       -moz-transition: all 0.3s ease-out;
        -ms-transition: all 0.3s ease-out;
         -o-transition: all 0.3s ease-out;
            transition: all 0.3s ease-out;
  }

  .hideBar {
    height: 50px;
    -webkit-transition: all 0.1s ease-out;
         -moz-transition: all 0.1s ease-out;
          -ms-transition: all 0.1s ease-out;
           -o-transition: all 0.1s ease-out;
              transition: all 0.1s ease-out;
  }
  .navbar-toggler{
    border: 2px solid #fff;
    color:#fff;
    font-size: 25px;
    padding:5px;
    padding-bottom:0px;
    z-index:1000;
  }

  .navbar-toggler:focus{
    border: 2px solid #fff;
  }
  .ml-auto{
    background-color: #727F80;
    padding-left: 50px;
    margin-top:-5px;
  }
  .navbar-brand {
    color: #fff;
  }
  .navbar-item ul li{
    color: #fff!important;
    cursor: pointer;
    padding-left: 10px;
    font-family: 'Comfortaa', cursive;
  }
  .nav-link{
    cursor:pointer;
    transition: 1s ease;
    color: #ffffff;
    text-decoration: none;
    border-top: 4px solid #727F80;
    border-bottom: 4px solid #727F80;
    padding: 3px 0;
  }

.nav-link:hover {
  border-top: 4px solid #ffffff;
  border-bottom: 4px solid #ffffff;
  padding: 3px 8px; 
}
@media screen and (max-width: 980px) {
  .navbar{
    border-bottom: 0px!important;
  }
}
</style>
