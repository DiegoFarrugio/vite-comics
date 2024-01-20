<script>
export default {
  data(){
    return{
        links: [
          'Characters',
          'Comics',
          'Movies',
          'TV',
          'Games',
          'Collectibles',
          'Videos',
          'Fans',
          'New',
          'Shop'
        ]
    }
  },

  methods: {}
}
</script>



<template>
  <header>

      <div id="container-header">
        <div class="display-flex-header">
          <div>
            <img src="/img/dc-logo.png" alt="">
          </div>
          <div>
            <ul class="display-flex-header">
              <li v-for="(link, i) in links" :key="i">
                <a href="#"> {{link}} </a>
              </li>
            </ul>
          </div>
        </div>
      </div>

  </header>
</template>



<style lang="scss" scoped>
@use "../assets/scss/header.scss" as *;
</style>