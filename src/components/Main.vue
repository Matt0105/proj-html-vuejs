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

</style>