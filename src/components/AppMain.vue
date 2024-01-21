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

        series: [
  {
      "thumb": "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
      "price": "$19.99",
      "series": "Action Comics",
      "type": "comic book",
  },
  {
      "thumb": "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
      "price": "$3.99",
      "series": "American Vampire 1976",
      "type": "comic book",
  },
  {
      "thumb": "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
      "price": "$16.99",
      "series": "Aquaman",
      "type": "graphic novel",
  },
  {
      "thumb": "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
      "price": "$2.99",
      "series": "Batgirl",
      "type": "comic book",
  },
  {
      "thumb": "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
      "price": "$3.99",
      "series": "Batman",
      "type": "comic book",
  },
  {
      "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg",
      "price": "$2.99",
      "series": "Batman Beyond",
      "type": "comic book",
  },
  {
      "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg",
      "price": "$3.99",
      "series": "Batman/Superman",
      "type": "comic book",
  },
  {
      "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg",
      "price": "$4.99",
      "series": "Batman/Superman Annual",
      "type": "comic book",
  },
  {
      "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg",
      "price": "$5.99",
      "series": "Batman: The Joker War Zone",
      "type": "comic book",
  },
  {
      "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg",
      "price": "$6.99",
      "series": "Batman: Three Jokers",
      "type": "comic book",
  },
  {
      "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg",
      "price": "$4.99",
      "series": "Batman: White Knight Presents: Harley Quinn",
      "type": "comic book",
  },
  {
      "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg",
      "price": "$16.99",
      "series": "Catwoman",
      "type": "graphic novel",
  }
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
    </div>
  </section>  

  <section id="main-section-2">
    <div v-for="(singleSeries, i) in series" :key="i" class="series_container single_series">
        <div>
            <img :src="singleSeries.thumb" alt="series.series">
        </div>
        <div>
            {{ singleSeries.series }}
        </div>
    </div>

    <div class="load-more-link">
        <a href="">
          LOAD MORE
        </a>
      </div>
  </section>

  <section>
    <div id="main-section-3">
      <div>
        <ul class="display-flex-main-section-3">
          <li v-for="(option, i) in options" :key="i">
            <img :src="option.img" alt="">
            <span> {{option.text}} </span>
          </li>
        </ul>
      </div>
    </div>
  </section>

  <section>
    <div id="main-section-4">
      <div class="display-flex-main-section-4">
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
