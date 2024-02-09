<script>

    export default{

        name: "MainSection"
    }

</script>

<template>
        <!-- CONTAINER CONTENT BLACK -->
    <div class="container-content">
        <div>
            <h4 class="text-white">
            -- content goes here --
            </h4>
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
    height: 100px;

    background-color: #1C1C1C;
}

.text-white{
    width: 80%;
    margin: 0 auto;
    padding-top: 40px;

    color: white;
    text-transform: capitalize;
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

</style>