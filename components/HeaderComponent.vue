<template>
  <div class="main">
    <div class="header">
      <div class="container">
        <nav class="navbar navbar-expand-lg navbar-light bg-faded" style="background-color: #e3f2fd;">
          <a class="navbar-brand" href="#">SUKANTA BALA</a>
          <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarTogglerDemo01" aria-controls="navbarTogglerDemo01" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
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
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .header{
    background-color: #e3f2fd;
    padding: 15px 0px;
  }
  .container {
    padding-right: 0px;
    padding-left: 0px;
  }
  .navbar-item ul li{
    cursor: pointer;
  }
  .nav-link{
    cursor:pointer;
  }
</style>
