<template>
  <div class="main">
    <navbar></navbar>
    <Slider></Slider>
    <div id="pageBody">
      <nuxt/>
    </div>
    <Footerbar></Footerbar>
  </div>
</template>

<script>
import Navbar from '~/components/HeaderComponent.vue'
import Slider from '~/components/Slider.vue'
import Footerbar from '~/components/FooterComponent.vue'

export default {
  components: {
    Navbar,
    Slider,
    Footerbar
  }
}
</script>
