<template>
  <div id="contact">
    <Header title="Oops! You seem to be lost :)" :small-header="true"/>
    <div class="max-width">
        <router-link :to="button.link" class="main-button">
            <span class="main-button--text">{{button.text}}</span> 
            <span class="main-button--icon">
              <svg version="1.1" id="Layer_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px" y="0px" viewBox="0 0 7.4 12" style="enable-background:new 0 0 7.4 12;" xml:space="preserve">
                <path class="st0" d="M1.4,0L0,1.4L4.6,6L0,10.6L1.4,12l6-6L1.4,0z"/>
              </svg>
            </span>
          </router-link>
    </div>
  </div>
</template>

<script>
import Header from '@/components/Header.vue'

export default {
  name: '404',
  data() {
      return {
          button:{
              link: '/',
              text: 'Take me home'
          }
      }
  },
  components: {
    Header,
  }
}
</script>
