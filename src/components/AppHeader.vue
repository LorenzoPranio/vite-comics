<script>
export default {
    
}
</script>

<template>
    <div>
        <div class="container">
            <div class="row">
                <div class="col-4 justify-content-start align-self-center p-4">
                    <img src="../assets/dc-logo.png" alt="">
                </div>
                <div class="col-8 justify-content-end align-self-center p-4">
                    <ul class="list-unstyled fw-bold">
                        <li><a href="#">CHARACTERS</a></li>
                        <li><a href="#">COMICS</a></li>
                        <li><a href="#">MOVIE</a></li>
                        <li><a href="#">TV</a></li>
                        <li><a href="#">GAMES</a></li>
                        <li><a href="#">COLLECTIBLES</a></li>
                        <li><a href="#">VIDEOS</a></li>
                        <li><a href="#">FANS</a></li>
                        <li><a href="#">NEWS</a></li>
                        <li><a href="#">SHOP</a></li>
                    </ul>
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables.scss';
    ul{
        display: flex;

        li{
            margin: 0px 15px;

            a{
                text-decoration: none;
                color: rgb(0, 0, 0);
                padding-bottom: 50px;

                &:hover{
                    border-bottom: 5px solid variables.$primary-color;
                    color: variables.$primary-color;
                }
            }

        }
    }
</style>