<template>
  <header>
      <div class="header-container">
        <NavBar />
        <div class="jumbo">
            <div class="head-jumbo">
                <h1>Learn At Your Own Pace!</h1>
                <p>Get teamed Up with people of the same will.</p>
                <button>Get started for free</button>
            </div>
            
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
    .header-container {
        width: 90%;
        height: 100%;
        margin: 0 auto;

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
                padding: 1rem;
                border: none;
                border-radius: 5px;
                color: white;
                font-weight: 600;
                background-color: #27ab94;
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