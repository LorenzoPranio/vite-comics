<script>
export default {
    
}
</script>

<template>
    <div>
        <div class="bg-img">
            <div class="container">
                <div class="row">
                    <div class="col-6 py-5">
                        <div class="col">
                            <div class="content">
                                <h4>DC COMICS</h4>
                                <ul class="text-secondary list-unstyled">
                                    <li>Characters</li>
                                    <li>Comics</li>
                                    <li>Movies</li>
                                    <li>TV</li>
                                    <li>Games</li>
                                    <li>Videos</li>
                                    <li>News</li>
                                </ul>
                            </div>
                            <div class="content">
                                <h4>SHOP</h4>
                                <ul class="text-secondary list-unstyled">
                                    <li>Shop DC</li>
                                    <li>Shop DC Collectibles</li>
                                </ul>
                            </div>
                        </div>
                        <div class="col">
                            <div class="content">
                                <h4>DC</h4>
                                <ul class="text-secondary list-unstyled">
                                    <li>Terms Of Use</li>
                                    <li>Privacy policy(New)</li>
                                    <li>Ad Choices</li>
                                    <li>Jobs</li>
                                    <li>Subscriptions</li>
                                    <li>Talent Workshops</li>
                                    <li>CPSC Certificates</li>
                                    <li>Ratings</li>
                                    <li>Shop Help</li>
                                    <li>Contact us</li>
                                </ul>
                            </div>
                        </div>
                        <div class="col">
                            <div class="content">
                                <h4>SITES</h4>
                                <ul class="text-secondary list-unstyled">
                                    <li>DC</li>
                                    <li>MAD Magazine</li>
                                    <li>DC Kids</li>
                                    <li>DC Universe</li>
                                    <li>DC Power Visa</li>
                                </ul>
                            </div>
                        </div>
                    </div>
                    <div class="col-6"> 
                        <img class="logo" src="../assets/dc-logo-bg.png">
                    </div>
                </div>
            </div>
        </div>
        <div class="bg-footer p-4">
            <div class="container">
                <div class="row">
                    <div class="col-6 d-flex justify-content-start align-self-center">
                        <button><p>SIGN-UP NOW!</p></button>
                    </div>
                    <div class="col-6 d-flex justify-content-end align-self-center">
                        <p class="fw-bold t-blue d-inline-block">FOLLOW US</p>
                        <img src="../assets/footer-facebook.png">
                        <img src="../assets/footer-twitter.png">
                        <img src="../assets/footer-youtube.png">
                        <img src="../assets/footer-pinterest.png">
                        <img src="../assets/footer-periscope.png">
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables.scss';

.bg-img{
    background-image: url(../assets/footer-bg.jpg);
    background-size: cover;
    overflow: hidden;
    position: relative;

    .col-6{
        display: flex;

        h4{
            color: variables.$white-color;
        }

        .logo{
            position: absolute;
            z-index: 2;
            width: 550px;
            top: 50%;
            left: 70%;
            transform: translate(-50%, -50%);
        }
    }
}
.bg-footer{
    background-color:rgb(70, 70, 70);
    z-index: 1;
    button{
        background-color: transparent;
        border: 3px solid variables.$primary-color;
        padding: 10px 15px;
        p{
            margin: 0px;
            color:  variables.$white-color;
        }
    }
    .t-blue{
        color: variables.$primary-color;
        margin: 0px;
        font-size: 20px;
    }
    img{
        margin: 0px 10px;
    }
}
    
</style>