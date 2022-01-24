<template>
  <main>
      <div class="container">

          <div class="motto-data">
              <div class="motto-container">
                  <p class="motto">Let passion and determination be the guide along the way and develop at your own pace that's comfortable.</p>
                  <h4>Fannie Moreno</h4>
                  <p class="ceo">/Founder & CEO</p>
              </div>

              <div class="data-container">
                  <ul>
                      <li>
                          <h2>1.926</h2>
                          <p>finished sessions</p>
                      </li>
                      <li>
                          <h2>3.092+</h2>
                          <p>enrolled learners</p>
                      </li>
                      <li>
                          <h2>200</h2>
                          <p>online instructors</p>
                      </li>
                      <li>
                          <h2>100%</h2>
                          <p>satisfaction rate</p>
                      </li>
                  </ul>
              </div>
          </div>

          <!-- services content -->

          <div class="services-container">
              <div class="card-side">

                  <div class="first-col">
                    <div class="card">
                        <div class="card__desc">
                            <h3>Graphic Design</h3>
                            <p>Have a passion for graphics and arts? Show your talents with confidence and self-assertiveness.</p>
                        </div>
                        <div class="card__img">
                            <img src="../assets/images/home-6-service-image-01.png" alt="">
                        </div>
                    </div>

                    <div class="card">
                        <div class="card__img">
                            <img src="../assets/images/home-6-service-image-03.png" alt="">
                        </div>
                        <div class="card__desc">
                            <h3>Idea Discussion</h3>
                            <p>Get teamed up with the specialists who work and teach coding for years at famous universities.</p>
                        </div>
                    </div>
                  </div>

                  <div class="second-col">
                    <div class="card">
                        <div class="card__desc">
                            <h3>Business Administration</h3>
                            <p>Learners are encouraged to study the mechanism and structure of system administration.</p>
                        </div>
                        <div class="card__img">
                            <img src="../assets/images/home-6-service-image-02.png" alt="">
                        </div>
                    </div>

                    <div class="card">
                        <div class="card__img">
                            <img src="../assets/images/home-6-service-image-04.png" alt="">
                        </div>
                        <div class="card__desc">
                            <h3>Web Development</h3>
                            <p>Learn to start building a webpage from scratch. You decide your own space, course and speed.</p>
                        </div>
                    </div>
                  </div>
                  

              </div>
              <div class="desc-side">
                  
              </div>
          </div>

      </div>
  </main>
</template>

<script>
export default {
    name: "Main",
}
</script>

<style lang="scss" scoped>
@import "../assets/scss/partials/_commons.scss";

    main {
        background-image: url(../assets/images/background-pattern-grid-line.png);
        width: 100%;
        margin-top: 15rem;
    }

    .motto-data {
        width: 100%;

        .motto-container {
            width: 100%;
            text-align: center;

            
            .motto {
                width: 55%;
                margin: auto;
                font-weight: 500;
                font-size: 2.5rem;
            }

            h4 {
                margin-top: 2rem;
                margin-bottom: 1rem;
                text-transform: uppercase;
            }

            p:not(.motto) {
                color: #9da1aa;
                font-size: 0.8rem;
            }
            
        }

        .data-container {

            margin-top: 5rem;

            ul {
                display: flex;
                justify-content: space-between;

                li {
                    display: flex;
                    flex-direction: column;
                    align-items: center;

                    h2 {
                        color: #1fad96;
                        font-size: 3rem;
                        font-weight: 700;
                    }

                    p {
                        text-transform: uppercase;
                        font-weight: 600;
                        letter-spacing: 1px;
                        color: #6c6c6c;
                    }
                }
            }
            

        }
    }

    .services-container {

        margin-top: 7rem;

        .card-side {
            width: 50%;
            display: flex;
            
            .card {
                display: flex;
                flex-direction: column;
                justify-content: space-between;
                height: 370px;
                width: 290px;
                padding-top: 1rem;
                background-color: white;
                margin-bottom: 2rem;
                box-shadow: 1px 2px 20px rgba(0,0,0,0.1);

                .card__desc {
                    padding: 1rem 1rem 1.2rem 1rem;

                    h3 {
                        font-weight: 600;
                    }
                    p {
                        color: #616865;
                        font-size: 0.9rem;
                        line-height: 25px;
                        margin-top: 0.6rem;
                    }
                }

                .card__img {
                    img {
                        display: block;
                        // padding-top: 1rem;
                    }
                }

            }

            .first-col {
                margin-right: 30px;
            }

            .second-col {
                position: relative;
                top: 80px;
                .card {
                    align-items: center;
                }
            }
        }

        
    }

</style>