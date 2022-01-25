<template>
  <header>
      <div class="container">
        <NavBar />
        <div class="jumbo">
            <div class="head-jumbo">
                <h1>Learn At Your Own Pace!</h1>
                <p>Get teamed Up with people of the same will.</p>
                <button class="main-btn" >Get started for free</button>
            </div>
            
            <!-- provare a inserire le due immagini all'interno di jumbo-imgs e spostarle con un position absolute -->
            <div class="jumbo-imgs"> 
                <img class="secondary-first" src="../assets/images/home-6-hero-left-person.png" alt="">
                <div class="jumbo-poster">
                    <img src="../assets/images/home-6-hero-poster-final.jpg" alt="">
                    <img class="yt-logo" src="../assets/images/icon-youtube-play.png" alt="">
                </div>
                <img class="secondary-second" src="../assets/images/home-6-hero-right-person-195x300.png" alt="">
            </div>
        </div>
      </div>
  </header>
</template>

<script>
import NavBar from "./NavBar.vue";

export default {
    name: "Header",
    components: {
        NavBar,
    }
}
</script>

<style lang="scss" scoped>
@import "../assets/scss/partials/_commons.scss";

    header {
        width: 100%;
        // height: 780px;
        // background-image: url("../assets/images/jumbotron-background-wave-big.svg");
        background-color: #1f2154;
        color: white;
    }
    .container {
        

        .jumbo {
            position: relative;
            width: 100%;
            text-align: center;
            // margin-top: 4rem;
            overflow: hidden;
            transform: translateY(100px);


            h1 {
                font-weight: 500;
                font-size: 3rem;
            }

            p {
                color: #f6f3f6;
                opacity: 0.8;
            }

            button {
                margin-top: 1.5rem;
                
            }

            .jumbo-imgs {
                width: 100%;
                display: flex;
                justify-content: center;
                align-items: center;

                .jumbo-poster {
                    position: relative;
                    bottom: 20px;
                    display: flex;
                    justify-content: center;
                    align-items: center;
                    width: 50%;
                    background-color: white;
                    border-radius: 20px;
                    margin-top: 5rem;
                    box-shadow: 2px 10px 10px rgba(128, 128, 128, 0.288);

                    img {
                        width: 95%;
                        margin: 1rem 0;
                    }

                    .yt-logo {
                        position: absolute;
                        top: 50%;
                        left: 50%;
                        transform: translate(-50%, -50%);
                        width: 100px;
                    }
                }

                .secondary-first, .secondary-second {
                    position: absolute;
                }
                .secondary-first {
                    left: 80px;
                    bottom: 0;
                }
                .secondary-second {
                    right: 14%;
                    bottom: -140px;
                }


            }
        }
        
    }
</style>