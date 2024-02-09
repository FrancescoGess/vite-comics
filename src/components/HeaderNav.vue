<script>
export default{
    name: "HeaderNav",
    data(){
        return{
            navLinks:[
                {
                    name: 'characthers',
                    current: false
                },
                {
                    name: 'comics',
                    current: true
                },
                {
                    name: 'movies',
                    current: false
                },
                {
                    name: 'tv',
                    current: false
                },
                {
                    name: 'games',
                    current: false
                },
                {
                    name: 'collectibles',
                    current: false
                },
                {
                    name: 'videos',
                    current: false
                },
                {
                    name: 'fans',
                    current: false
                },
                {
                    name: 'news',
                    current: false
                },
                {
                    name: 'shop',
                    current: false
                },
            ]
        }
    }
}
</script>

<template>

    <!-- LOGO -->
    <div class="container">
        <div class="container-pic">
            <figure>
                <img src="../assets/img/dc-logo.png" alt="logo header">
            </figure>
        </div>
    
                <!-- NAVBAR -->
        <div>
            <nav>
                <ul class="flex-nav">
                    <li v-for="(element, index) in navLinks"
                    :key="index"
                    :class="element.current ? 'active' : '' ">
                        <a href="#">{{element.name}}</a>
                    </li>
                    <!-- <li>
                        <a href="#">comics</a>
                    </li>
                    <li>
                        <a href="#">movies</a>
                    </li>
                    <li>
                        <a href="#">tv</a>
                    </li>
                    <li>
                        <a href="#">games</a>
                    </li>
                    <li>
                        <a href="#">collectibles</a>
                    </li>
                    <li>
                        <a href="#">videos</a>
                    </li>
                    <li>
                        <a href="#">fans</a>
                    </li>
                    <li>
                        <a href="#">news</a>
                    </li>
                    <li>
                        <a href="#">shop</a>
                    </li> -->
                </ul>
            </nav>
        </div>
    </div>


</template>

<style scoped>
.active{
    color: #3C8EF9;
}

.container{
    display: flex;
    justify-content: space-between;

    width: 80%;
    margin: 0 auto;
    padding-top: 20px;
    align-items: center;
    
}


.flex-nav{
    display: flex;
    gap: 10px;
}

.flex-nav li{
    text-transform: uppercase;
    list-style-type: none;
    font-weight: bold;
}

.flex-nav li a {
    text-decoration: none;
    color: gray;
}

.flex-nav li a:hover{
    color: #3C8EF9;
}

.flex-nav li a::after{
    content: '';
    display: block;
    width: 0;
    height: 2px;
    background: #3C8EF9;
    transition: width .3s;
}

.flex-nav li a:hover::after{
    width: 100%;
    transition: width .9s;
}
</style>