<script>

    import CardFumetti from './CardFumetti.vue';

    export default {
        name: 'MainSection',
        components: {
            CardFumetti
        },
        data () {
            return {
                cardItems: [
{
      "thumb": "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
      "price": "$19.99",
      "series": "Action Comics",
      "type": "comic book"
  },
  {
      "thumb": "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
      "price": "$3.99",
      "series": "American Vampire 1976",
      "type": "comic book"
  },
  {
      "thumb": "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
      "price": "$16.99",
      "series": "Aquaman",
      "type": "graphic novel"
  },
  {
      "thumb": "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
      "price": "$2.99",
      "series": "Batgirl",
      "type": "comic book"
  },
  {
      "thumb": "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
      "price": "$3.99",
      "series": "Batman",
      "type": "comic book"
  },
  {
      "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg",
      "price": "$2.99",
      "series": "Batman Beyond",
      "type": "comic book"
  },
  {
      "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg",
      "price": "$3.99",
      "series": "Batman/Superman",
      "type": "comic book"
  },
  {
      "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg",
      "price": "$4.99",
      "series": "Batman/Superman Annual",
      "type": "comic book"
  },
  {
      "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg",
      "price": "$5.99",
      "series": "Batman: The Joker War Zone",
      "type": "comic book"
  },
  {
      "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg",
      "price": "$6.99",
      "series": "Batman: Three Jokers",
      "type": "comic book"
  },
  {
      "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg",
      "price": "$4.99",
      "series": "Batman: White Knight Presents: Harley Quinn",
      "type": "comic book"
  },
  {
      "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg",
      "price": "$16.99",
      "series": "Catwoman",
      "type": "graphic novel"
  }
]
                
    
        }},
    }


</script>

<template>
        <!-- CONTAINER CONTENT BLACK -->
    <div class="container-content">
        <div class="position-series">
            <h4 class="text-white">
            current series
            </h4>
        </div>

        <div class="cards">
            <CardFumetti v-for="(element, index) in cardItems"
            :key="index"
            :props-thumb="element.thumb"
            :props-series="element.series">

            </CardFumetti>
        </div>
    </div>

        <!-- CONTAINER CONTENT BLUE -->
    <div class="container-digital-comics">
        <div class="flex-items">
          <figure>
            <img src="../assets/img/buy-comics-merchandise.png" style=" width: 50px;" alt="">
        </figure>
        <span>
            digital comics
        </span>
          <figure>
            <img src="../assets/img/buy-comics-digital-comics.png" style=" width: 40px;" alt="">
        </figure>
        <span>
            merchandise
        </span>
          <figure>
            <img src="../assets/img/buy-comics-shop-locator.png" style=" width: 35px;" alt="">
        </figure>
        <span>
            subscription
        </span>
          <figure>
            <img src="../assets/img/buy-comics-subscriptions.png" style=" width: 50px;" alt="">
        </figure>
        <span>
            comic shop locator
        </span>
          <figure>
            <img src="../assets/img/buy-dc-power-visa.svg" style=" width: 50px;" alt="">
        </figure>
        <span>
            dc power visa
        </span>
        </div>
    </div>

</template>

<style>

.container-content{
    height: 100%;

    background-color: #1C1C1C;
}

.text-white{
    margin: 0 auto;
    padding: 15px;

    background-color: #0282F9;
    color: white;

    text-transform: uppercase;

    position: absolute;
    bottom: -25px;
    left: 150px;
}


.position-series{
    position: relative;
}

.container-digital-comics{
    background-color: #0282F9;
    height: 150px;

    display: flex;
}

.flex-items{
    margin: 0 auto;
    width: 60%;

    display: flex;
    gap: 20px;
    align-items: center;
}

.flex-items figure {
    padding-top: 20px;


    display: flex;
    align-items: center;
}

.flex-items span{
    color: white;
    text-transform: uppercase;
    padding-top: 2%;
}

.container-cards{
    width: 70%;
    display: flex;
    margin: 0 auto;

    border: 1px solid red;
    padding-top: 50px;
}

.cards{
    display: flex;
    flex-wrap: wrap;
    gap: 20px;

    margin: 0 auto;
    width: 80%;
} 

</style>