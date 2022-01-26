<template>
  <footer>
      <div class="container">
          <div class="links-container">
              <div class="address">
                    <h4>Address</h4>
                    <p>382 NE 191st St # 87394 Miami, FL 33179-3899</p>
                    <p>+1(305) 547-9909 (9am - 5pm EST, Monday - Friday)</p>
                    <p>support@maxcoach.com</p>

                    <ul class="social-links">
                        <li><a href=""><i class="fab fa-facebook-square"></i></a></li>
                        <li><a href=""><i class="fab fa-twitter"></i></a></li>
                        <li><a href=""><i class="fab fa-instagram"></i></a></li>
                        <li><a href=""><i class="fab fa-linkedin"></i></a></li>
                    </ul>
              </div>
              
              <div class="explore">
                  <h4>Explore</h4>
                  <div class="explore-links">
                    <div class="first-col">
                        <ul>
                            <li><a href="">Start here</a></li>
                            <li><a href="">Blog</a></li>
                            <li><a href="">About us</a></li>
                        </ul>
                    </div>
                    <div class="second-col">
                        <ul>
                            <li><a href="">Success story</a></li>
                            <li><a href="">Courses</a></li>
                            <li><a href="">Contact us</a></li>
                        </ul>
                    </div>

                </div>  
              </div>

              <div class="information">
                    <h4>Information</h4>
                    <ul>
                        <li><a href="">Membership</a></li>
                        <li><a href="">Purchase guide</a></li>
                        <li><a href="">Privacy policy</a></li>
                        <li><a href="">Terms of services</a></li>
                    </ul>
              </div>

          </div>

          <p class="copyright" >&copy; 2020 Maxcouach. All Rights Reserved</p>
      </div>
  </footer>
</template>

<script>
export default {
    name: "Footer",
}
</script>

<style lang="scss" scoped>
@import "../assets/scss/partials/_commons.scss";
@import "../assets/scss/partials/_variables.scss";

    footer {
        background-color: $hintRed;

        p, li, a {
            font-size: 0.8rem;
            color: $corduroy;
        }
        p:not(.copyright), li {
            margin: 0.8rem 0;
        }

        h4 {
            margin-top: 3rem;
            font-weight: 600;
        }

        .links-container {
            display: flex;
            width: 100%;

            .address {
                width: 50%;

                .social-links {
                    display: flex;

                    li {
                        margin-right: 1.5rem;

                        a {
                            font-size: 1.3rem;
                            color: $grayChateau;
                        }
                    }
                }
            }

            .explore {
                margin-right: 4rem;
                
                .explore-links {
                    display: flex;

                    .first-col {
                        margin-right: 3rem;
                    }
                }
            }
        }

        .copyright {
            padding: 2rem 0 3rem 0;
            text-align: center;
            color: $grayChateau;
        }
    }
</style>