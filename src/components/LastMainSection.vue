<script>

    export default{

        name: "LastMainSection",
        data(){
            return{
                footNavLink:[
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
                    name: 'videos',
                    current: false
                },
                {
                    name: 'news',
                    current: false
                }
                ]
            }
        }
    }

</script>


<template>

        <div class="bg-comics">
            <div class="container-first-sec">           
            <div class="container-dc-comics">
                <h4>
                    dc comics
                </h4>
                <ul>
                    <li v-for="(element, index) in footNavLink"
                    :key="index">
                        <a href="#">{{element.name}}</a>
                    </li>
                    <!-- <li>
                        <a href="#">comics</a>
                    </li>
                    <li>
                        <a href="#">Movies</a>
                    </li>
                    <li>
                        <a href="#">TV</a>
                    </li>
                    <li>
                        <a href="#">games</a>
                    </li>
                    <li>
                        <a href="#">videos</a>
                    </li>
                    <li>
                        <a href="#">news</a>
                    </li> -->
                </ul>

            <div class="container-shop">
                <h4>
                    shop
                </h4>
                <ul>
                    <li>
                        <a href="#">shop DC</a>
                    </li>
                    <li>
                        <a href="#">shop DC Collectibles</a>
                    </li>
                </ul>
            </div>
            </div>
        <div class="container-dc">
            <h4>
                dc
            </h4>
            <ul>
                <li>
                    <a href="#">Terms of Use</a>
                </li>
                <li>
                    <a href="#">privacy policy (New)</a>
                </li>
                <li>
                    <a href="#">ad choice</a>
                </li>
                <li>
                    <a href="#">advertising</a>
                </li>
                <li>
                    <a href="#">jobs</a>
                </li>
                <li>
                    <a href="#">subscription</a>
                </li>
                <li>
                    <a href="#">talent workshop</a>
                </li>
                <li>
                    <a href="#">CPSC Certificates</a>
                </li>
                <li>
                    <a href="#">ratings</a>
                </li>
                <li>
                    <a href="#">shop help</a>
                </li>
                <li>
                    <a href="#">contact us</a>
                </li>
            </ul>
        </div>
        <div class="container-dc-comics">
                <h4>
                    sites
                </h4>
                <ul>
                    <li>
                        <a href="#">DC</a>
                    </li>
                    <li>
                        <a href="#">MAD magazine</a>
                    </li>
                    <li>
                        <a href="#">DC Kids</a>
                    </li>
                    <li>
                        <a href="#">DC Universe</a>
                    </li>
                    <li>
                        <a href="#">DC power visa</a>
                    </li>
                </ul>
            </div>
        </div>
    </div>

</template>

<style>
.container-first-sec{
    margin-left: 20rem;

    width: 30%;
    display: flex;
    /* flex-direction: row; */
    gap: 40px;
}


.bg-comics{
    background-image: url(../assets/img/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    padding-top: 20px;
    
    height: 450px;
}


.container-shop{
    padding-top: 30px;
}

.container-dc-comics{
    
    li{
        list-style-type: none;
        margin-top: 8px;
        
        a{
            text-transform: capitalize;
            color: grey;
            text-decoration: none;
        }
    }
    
    h4{
        font-size: 20px;
        text-transform: uppercase;
        
        color: white;

    }
}

.container-dc{

            h4{
            font-size: 20px;
            text-transform: uppercase;
            
            color: white;
        }
        
        li{
            list-style-type: none;
            margin-top: 8px;
            
            a{
                text-transform: capitalize;
                color: grey;
                text-decoration: none;               
        }
    }
}

</style>