<script>

    export default{

        name: "CardFumetti",
        props: {
            propsThumb: String,
            propsSeries: String
        },
        data(){
            return{

            }
        }
    }

</script>

<template>
<div class="container-comics">

   <div class="card">
    <figure>
        <img :src="propsThumb" alt="">
    </figure>
    <h4>
        {{ propsSeries }}
    </h4>
   </div>
</div>
</template>

<style>

.card{
    flex-basis: calc( 100% / 6 - 20 ); 
}

.card figure img{
    width: 100%;
    display: block;
}


.container-comics{

    flex-basis: calc( 100% / 6 - 20px);
}
</style>