<script>
export default {
  data(){
    return{
        options: [
        {
          img : "/img/buy-comics-digital-comics.png",
          text : 'DIGITAL COMIC'
        },

        {
          img : "/img/buy-comics-merchandise.png",
          text : 'DIGITAL COMIC'
        },

        {
          img : "/img/buy-comics-subscriptions.png",
          text : 'DIGITAL COMIC'
        },

        {
          img : "/img/buy-comics-shop-locator.png",
          text : 'DIGITAL COMIC'
        },

        {
          img : "/img/buy-dc-power-visa.svg",
          text : 'DIGITAL COMIC'
        },

        ],

        dcComics: [
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
        ],

        shop: [
          'Shop DC',
          'Shop DC Collectibles', 
        ],

        dc: [
          'Terms Of Use',
          'Privacy Policy',
          'Ad Choices',
          'Advertising',
          'Jobs',
          'Subscription',
          'Talent Workshop',
          'CPSC Certificates',
          'Raitings',
          'Shop Help',
          'Contact Us',
        ],

        site: [
          'DC',
          'MAD Magazine',
          'DC Kids',
          'DC Universe',
          'DC Power Visa'
        ],
    }
  },

  methods: {}
}
</script>



<template>
  <div class="container">

  <section>
    <div id="main-section-1">
      <h2> -->Contents goes here <-- </h2>
    </div>
  </section>  

  <section>
    <div id="main-section-2">
      <div>
        <ul class="display-flex-main-section-2">
          <li v-for="(option, i) in options" :key="i">
            <img :src="option.img" alt="">
            <span> {{option.text}} </span>
          </li>
        </ul>
      </div>
    </div>
  </section>

  <section>
    <div id="main-section-3">
      <div class="display-flex-main-section-3">
        <div class="list-1">
          <h3>DC COMICS</h3>
            <ul>
              <li v-for="(choice, i) in dcComics" :key="i">
                {{ choice }}
              </li>
            </ul>
          
          <h3>
            SHOP
          </h3>
            <ul>
              <li v-for="(shops, i) in shop">
                {{ shops }}
              </li>
            </ul>
        </div>


        <div class="list-2">
          <h3>
            DC
          </h3>
            <ul>
              <li v-for="(dcs, i) in dc" :key="i">
                {{ dcs }}
              </li>
            </ul>
        </div>

        <div class="list-3">
          <h3>
            SITES
          </h3>
            <ul>
              <li v-for="(sites, i) in site" :key="i">
                {{ sites }}
              </li>
            </ul>
        </div>
      </div>

    </div>
  </section>
  
</div>
</template>



<style lang="scss" scoped>
@use "../assets/scss/main.scss" as *;
</style>
