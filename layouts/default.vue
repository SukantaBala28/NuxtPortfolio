<template>
  <div class="main">
    <navbar></navbar>
    <div id="pageBody">
      <nuxt/>
    </div>
    <Footerbar></Footerbar>
  </div>
</template>

<script>
import Navbar from '~/components/HeaderComponent.vue'
import Footerbar from '~/components/FooterComponent.vue'

export default {
  components: {
    Navbar,
    Footerbar
  }
}
</script>
