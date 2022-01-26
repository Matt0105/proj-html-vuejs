<template>
  <header>
      <div class="container">
        <NavBar />
        <div class="side-menu">
            <ul>
                <li><a href=""><img src="../assets/images/ruler-svgrepo-com.svg" alt=""></a></li>
                <li><a href=""><img src="../assets/images/life-buoy-svgrepo-com.svg" alt=""></a></li>
                <li><a href=""><img src="../assets/images/book-svgrepo-com.svg" alt=""></a></li>
                <li><a href=""><img src="../assets/images/cart-svgrepo-com.svg" alt=""></a></li>
            </ul>
        </div>
        <div class="jumbo">
            <div class="head-jumbo">
                <h1>Learn At Your Own Pace!</h1>
                <p>Get teamed Up with people of the same will.</p>
                <button class="main-btn" >Get started for free</button>
            </div>
            
            <!-- provare a inserire le due immagini all'interno di jumbo-imgs e spostarle con un position absolute -->
            <div class="jumbo-imgs"> 
                <div class="jumbo-poster">
                    <img class="secondary-first" src="../assets/images/home-6-hero-left-person.png" alt="">
                    <img class="preview" src="../assets/images/home-6-hero-poster-final.jpg" alt="">
                    <img class="yt-logo" src="../assets/images/icon-youtube-play.png" alt="">
                    <img class="secondary-second" src="../assets/images/home-6-hero-right-person-195x300.png" alt="">
                </div>
            </div>
        </div>
      </div>
      
    <svg id="wave" style="transform:rotate(0deg); transition: 0.3s" viewBox="0 0 1440 490" version="1.1" xmlns="http://www.w3.org/2000/svg"><defs><linearGradient id="sw-gradient-0" x1="0" x2="0" y1="1" y2="0"><stop stop-color="rgba(31, 33, 84, 0)" offset="0%"></stop><stop stop-color="rgba(248.597, 248.597, 248.597, 1)" offset="100%"></stop></linearGradient></defs><path style="transform:translate(0, 0px); opacity:1" fill="url(#sw-gradient-0)" d="M0,441L34.3,383.8C68.6,327,137,212,206,212.3C274.3,212,343,327,411,343C480,359,549,278,617,245C685.7,212,754,229,823,204.2C891.4,180,960,114,1029,122.5C1097.1,131,1166,212,1234,220.5C1302.9,229,1371,163,1440,187.8C1508.6,212,1577,327,1646,367.5C1714.3,408,1783,376,1851,375.7C1920,376,1989,408,2057,367.5C2125.7,327,2194,212,2263,138.8C2331.4,65,2400,33,2469,73.5C2537.1,114,2606,229,2674,261.3C2742.9,294,2811,245,2880,245C2948.6,245,3017,294,3086,334.8C3154.3,376,3223,408,3291,359.3C3360,310,3429,180,3497,155.2C3565.7,131,3634,212,3703,228.7C3771.4,245,3840,196,3909,163.3C3977.1,131,4046,114,4114,147C4182.9,180,4251,261,4320,269.5C4388.6,278,4457,212,4526,220.5C4594.3,229,4663,310,4731,294C4800,278,4869,163,4903,106.2L4937.1,49L4937.1,490L4902.9,490C4868.6,490,4800,490,4731,490C4662.9,490,4594,490,4526,490C4457.1,490,4389,490,4320,490C4251.4,490,4183,490,4114,490C4045.7,490,3977,490,3909,490C3840,490,3771,490,3703,490C3634.3,490,3566,490,3497,490C3428.6,490,3360,490,3291,490C3222.9,490,3154,490,3086,490C3017.1,490,2949,490,2880,490C2811.4,490,2743,490,2674,490C2605.7,490,2537,490,2469,490C2400,490,2331,490,2263,490C2194.3,490,2126,490,2057,490C1988.6,490,1920,490,1851,490C1782.9,490,1714,490,1646,490C1577.1,490,1509,490,1440,490C1371.4,490,1303,490,1234,490C1165.7,490,1097,490,1029,490C960,490,891,490,823,490C754.3,490,686,490,617,490C548.6,490,480,490,411,490C342.9,490,274,490,206,490C137.1,490,69,490,34,490L0,490Z"></path></svg>

    <svg id="wave2" style="transform:rotate(0deg); transition: 0.3s" viewBox="0 0 1440 490" version="1.1" xmlns="http://www.w3.org/2000/svg"><defs><linearGradient id="sw-gradient-0" x1="0" x2="0" y1="1" y2="0"><stop stop-color="rgba(31, 33, 84, 0)" offset="0%"></stop><stop stop-color="rgba(248.597, 248.597, 248.597, 1)" offset="100%"></stop></linearGradient></defs><path style="transform:translate(0, 0px); opacity:1" fill="url(#sw-gradient-0)" d="M0,441L17.1,383.8C34.3,327,69,212,103,212.3C137.1,212,171,327,206,343C240,359,274,278,309,245C342.9,212,377,229,411,204.2C445.7,180,480,114,514,122.5C548.6,131,583,212,617,220.5C651.4,229,686,163,720,187.8C754.3,212,789,327,823,367.5C857.1,408,891,376,926,375.7C960,376,994,408,1029,367.5C1062.9,327,1097,212,1131,138.8C1165.7,65,1200,33,1234,73.5C1268.6,114,1303,229,1337,261.3C1371.4,294,1406,245,1440,245C1474.3,245,1509,294,1543,334.8C1577.1,376,1611,408,1646,359.3C1680,310,1714,180,1749,155.2C1782.9,131,1817,212,1851,228.7C1885.7,245,1920,196,1954,163.3C1988.6,131,2023,114,2057,147C2091.4,180,2126,261,2160,269.5C2194.3,278,2229,212,2263,220.5C2297.1,229,2331,310,2366,294C2400,278,2434,163,2451,106.2L2468.6,49L2468.6,490L2451.4,490C2434.3,490,2400,490,2366,490C2331.4,490,2297,490,2263,490C2228.6,490,2194,490,2160,490C2125.7,490,2091,490,2057,490C2022.9,490,1989,490,1954,490C1920,490,1886,490,1851,490C1817.1,490,1783,490,1749,490C1714.3,490,1680,490,1646,490C1611.4,490,1577,490,1543,490C1508.6,490,1474,490,1440,490C1405.7,490,1371,490,1337,490C1302.9,490,1269,490,1234,490C1200,490,1166,490,1131,490C1097.1,490,1063,490,1029,490C994.3,490,960,490,926,490C891.4,490,857,490,823,490C788.6,490,754,490,720,490C685.7,490,651,490,617,490C582.9,490,549,490,514,490C480,490,446,490,411,490C377.1,490,343,490,309,490C274.3,490,240,490,206,490C171.4,490,137,490,103,490C68.6,490,34,490,17,490L0,490Z"></path></svg>

    <svg id="wave3" style="transform:rotate(0deg); transition: 0.3s" viewBox="0 0 1440 490" version="1.1" xmlns="http://www.w3.org/2000/svg"><defs><linearGradient id="sw-gradient-0" x1="0" x2="0" y1="1" y2="0"><stop stop-color="rgba(31, 33, 84, 0)" offset="0%"></stop><stop stop-color="rgba(248.597, 248.597, 248.597, 1)" offset="100%"></stop></linearGradient></defs><path style="transform:translate(0, 0px); opacity:1" fill="url(#sw-gradient-0)" d="M0,98L34.3,138.8C68.6,180,137,261,206,302.2C274.3,343,343,343,411,285.8C480,229,549,114,617,122.5C685.7,131,754,261,823,269.5C891.4,278,960,163,1029,98C1097.1,33,1166,16,1234,49C1302.9,82,1371,163,1440,187.8C1508.6,212,1577,180,1646,163.3C1714.3,147,1783,147,1851,196C1920,245,1989,343,2057,343C2125.7,343,2194,245,2263,228.7C2331.4,212,2400,278,2469,261.3C2537.1,245,2606,147,2674,106.2C2742.9,65,2811,82,2880,130.7C2948.6,180,3017,261,3086,294C3154.3,327,3223,310,3291,294C3360,278,3429,261,3497,212.3C3565.7,163,3634,82,3703,73.5C3771.4,65,3840,131,3909,179.7C3977.1,229,4046,261,4114,294C4182.9,327,4251,359,4320,359.3C4388.6,359,4457,327,4526,334.8C4594.3,343,4663,392,4731,359.3C4800,327,4869,212,4903,155.2L4937.1,98L4937.1,490L4902.9,490C4868.6,490,4800,490,4731,490C4662.9,490,4594,490,4526,490C4457.1,490,4389,490,4320,490C4251.4,490,4183,490,4114,490C4045.7,490,3977,490,3909,490C3840,490,3771,490,3703,490C3634.3,490,3566,490,3497,490C3428.6,490,3360,490,3291,490C3222.9,490,3154,490,3086,490C3017.1,490,2949,490,2880,490C2811.4,490,2743,490,2674,490C2605.7,490,2537,490,2469,490C2400,490,2331,490,2263,490C2194.3,490,2126,490,2057,490C1988.6,490,1920,490,1851,490C1782.9,490,1714,490,1646,490C1577.1,490,1509,490,1440,490C1371.4,490,1303,490,1234,490C1165.7,490,1097,490,1029,490C960,490,891,490,823,490C754.3,490,686,490,617,490C548.6,490,480,490,411,490C342.9,490,274,490,206,490C137.1,490,69,490,34,490L0,490Z"></path></svg>
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
@import "../assets/scss/partials/_variables.scss";

    header {
        position: relative;
        width: 100%;
        background-color: $portGore;
        color: white;

        #wave {
            position: absolute;
            bottom: 0;
            left: 0;
            opacity: 0.05;
        }
        #wave2 {
            position: absolute;
            bottom: 0;
            opacity: 0.07;

        }
        #wave3 {
            position: absolute;
            bottom: 10px;
            opacity: 0.02;
        }
    }

    .side-menu {
        position: absolute;
        top: 210px;
        right: 0;
        background-color: white;
        border-top-left-radius: 5px;
        border-bottom-left-radius: 5px;
        z-index: 150;

        ul {
            padding: 0.2rem;

            li{
                padding: 0.3rem;

                img {
                    width: 18px;
                    cursor: pointer;
                }
            }
        }
    }

    .jumbo {
        position: relative;
        width: 100%;
        text-align: center;
        overflow: hidden;
        transform: translateY(100px);
        z-index: 101;

        h1 {
            font-weight: 500;
            font-size: 3rem;
        }

        p {
            color: $hintRed;
            opacity: 0.8;
        }

        button {
            margin-top: 1.5rem;

            &:hover {
                background-color: white;
                color: $jungleGreen;
            }
        }

        .jumbo-imgs {
            display: flex;
            justify-content: center;
            align-items: center;
            width: 100%;
            z-index: 110;

            .jumbo-poster {
                position: relative;
                bottom: 20px;
                display: flex;
                justify-content: center;
                align-items: center;
                width: 50%;
                margin-top: 5rem;
                border-radius: 20px;
                box-shadow: 2px 10px 10px rgba(128, 128, 128, 0.288);
                background-color: white;

                .preview {
                    width: 95%;
                    margin: 1rem 0;
                }

                .secondary-first {
                    position: absolute;
                    bottom: 0;
                    left: -50%;
                    z-index: -100;
                }

                .secondary-second {
                    position: absolute;
                    bottom: -150px;
                    right: -200px;
                }

                .yt-logo {
                    position: absolute;
                    top: 50%;
                    left: 50%;
                    transform: translate(-50%, -50%);
                    width: 100px;
                }
            }
        }
    }
</style>