<script>
import comics from '../data/dc-comics.json'
export default {
    data(){
        return{
            comics
        }
    }
}
</script>

<template>
    <div>
        <div class="bg-teentitans">
            <span class="badge"><h4 class="fw-bold">CURRENT SERIES</h4></span>
        </div>
        <div class="bg-dark">
            <div class="container">
                <div class="row">
                    <div class="col-12 p-2 d-flex flex-wrap justify-content-center mt-3">
                        <div v-for="(comic, index) in comics" :key="index" class="col-2 d-flex">
                            <div class="card m-2">
                                <img :src="comic.thumb" :alt="comic.series" class="card-img-top img-fluid">
                                <div>
                                    <p class="text-center">{{ comic.series }}</p>
                                </div>
                            </div>
                        </div>
                        <div>
                            <button class="btn btn-primary"><p class="fw-bold">LOAD MORE</p></button>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="bg-azure p-5">
            <div class="container">
                <div class="row justify-content-evenly">
                    <div class="col-2 align-self-center">
                        <img src="../assets/buy-comics-digital-comics.png">
                        <p class="d-inline-block">DIGITAL COMICS</p>
                    </div>
                    <div class="col-2 align-self-center">
                        <img src="../assets/buy-comics-merchandise.png">
                        <p class="d-inline-block">DC MERCHANDISE</p>
                    </div>
                    <div class="col-2 align-self-center">
                        <img src="../assets/buy-comics-subscriptions.png">
                        <p class="d-inline-block">SUBSCRIPTION</p>
                    </div>
                    <div class="col-2 align-self-center">
                        <img src="../assets/buy-comics-shop-locator.png">
                        <p class="d-inline-block">COMIC SHOP LOCATOR</p>
                    </div>
                    <div class="col-2 align-self-center">
                        <img src="../assets/buy-dc-power-visa.svg">
                        <p class="d-inline-block">DC POWER VISA</p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables.scss';

.col-12{
    h1{
        color: variables.$white-color;
    }
}
.bg-azure{
    background-color: variables.$primary-color;
    .col-2{
        justify-content: center;
        padding: 0px;
        img{
            max-width: 75px;
            max-height: 75px;
            margin-right: 10px;
        }
        p{
            color: variables.$white-color;
        }
    }
}
.bg-teentitans{
    background-image: url(../assets/jumbotron.jpg);
    background-size: cover;
    height: 450px;
    position: relative;
    .badge{
        position: absolute;
        bottom: -22px;
        left: 150px;
        background-color: variables.$primary-color;
        border-radius: 0px;
        padding: 8px 25px;
        h4{
            margin: 0px;
        }
    }
}
.card{
    background-color: transparent;
    border: none;
    color: variables.$white-color;
    img{
        width: 175px;
        height: 205px;
        margin: 10px;
    }
    p{
        margin: 0px;
    }
}
.btn-primary{
    color: variables.$white-color;
    background-color: variables.$primary-color;
    border-radius: 0px;
    padding: 8px 60px;
    margin-top: 20px;
    p{
        margin: 0px;
    }
}
</style>