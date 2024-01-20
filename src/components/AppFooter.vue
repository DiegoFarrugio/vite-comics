<script>
export default {
  data(){
    return{
        logoImg : [
        "/img/footer-facebook.png",
        "/img/footer-twitter.png",
        "/img/footer-pinterest.png",
        "/img/footer-youtube.png",
        "/img/footer-periscope.png"
        ]
    }
  },

  methods: {}
}
</script>



<template>
  <footer>
    <div class="display-flex-footer">
      <div class="button-sing-up">
        <strong>SIGN-UP NOW!</strong>
      </div>

      <div class="display-flex-loghi-footer">
        <span><strong>FOLLOW US</strong></span>
        <div v-for="(logoImages, i) in logoImg" :key="i">
          <img :src="logoImages" alt="">
        </div>
      </div>

    </div>
  </footer>
</template>



<style lang="scss" scoped>
@use "../assets/scss/footer.scss" as *;
</style>
