<script>

    export default{

        name: "FooterContact"
    }

</script>

<template>

    <div class="footer-contact">
        <div class="flex-elements">
            <div class="container-btn">
                <button>
                    <a href="#">sign up now!</a>
                </button>
            </div>
            <div class="container-social">
                <div class="flex-social">
                    <span>
                        follow us
                    </span>
                        <figure>
                            <a href="#"><img src="../assets/img/footer-facebook.png" alt="facebook"></a>
                        </figure>
                        <figure>
                            <a href=""><img src="../assets/img/footer-twitter.png" alt="twitter"></a>
                        </figure>
                        <figure>
                            <a href=""><img src="../assets/img/footer-youtube.png" alt="youtube"></a>
                        </figure>
                        <figure>
                            <a href=""><img src="../assets/img/footer-pinterest.png" alt="pinterest"></a>
                        </figure>
                        <figure>
                            <a href=""><img src="../assets/img/footer-periscope.png" alt="periscope"></a>
                        </figure>                
                </div>
            </div>
        </div>
    </div>

</template>

<style>

    .footer-contact{
        background-color: #303030;
        width: 100%;
        height: 139px;
    }

    .flex-elements{
        width: 70%;
        height: 70%;
        padding-top: 50px;
        margin: 0 auto;

        display: flex;
        justify-content: space-between;
    }

    .container-btn{
        width: 150px;

        button{
            width: 100%;
            height: 100%;
            
            color: black;
            border: 2px solid #0282F9;

            background-color:  #303030;
        }
        a{
            text-decoration: none;
            color: white;
            text-transform: uppercase;
            padding: 10px;
        }
    }

    .container-social{
        width: 400px;

        .flex-social{
            display: flex;
            align-items: center;

            gap: 15px;
        }

        span{
            text-transform: uppercase;
            font-weight: bold;
            color: #0677d4;
        }
    }
</style>