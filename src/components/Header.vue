<template>
  <header>
      <div class="header-container">
        <nav>
          <div class="logo">
              <img src="../assets/images/light-logo.png" alt="">
          </div>
          <div class="navbar__menu-container">
              <ul class="navbar__menu">
                  <li><a href="#">Home<i class="fas fa-chevron-down"></i></a></li>
                  <li><a href="#">Pages<i class="fas fa-chevron-down"></i></a></li>
                  <li><a href="#">Courses<i class="fas fa-chevron-down"></i></a></li>
                  <li><a href="#">Features<i class="fas fa-chevron-down"></i></a></li>
                  <li><a href="#">Blog<i class="fas fa-chevron-down"></i></a></li>
                  <li><a href="#">Shop<i class="fas fa-chevron-down"></i></a></li>
                  <li><a href="#"><i class="fas fa-shopping-cart myArea"></i></a></li>
                  <li><a href="#"><i class="far fa-user-circle myArea"></i></a></li>
              </ul>

              <div class="input-container">
                  <input placeholder="Search..." type="text">
                  <i class="fas fa-search search"></i>
              </div>
          </div>
        </nav>
      </div>
      
  </header>
</template>

<script>
export default {
    name: "Header",
}
</script>

<style lang="scss" scoped>
@import "../assets/scss/partials/_commons.scss";

    header {
        width: 100%;
        height: 80px;
        // background-image: url("../assets/images/jumbotron-background-wave-big.svg");
        background-color: #1f2154;
        color: white;
    }
    .header-container {
        width: 80%;
        height: 100%;
        margin: 0 auto;

        nav {
            display: flex;
            width: 100%;
            height: 100%;
            justify-content: space-between;
            padding: 1rem 0;

            .logo {
                display: flex;
                align-items: center;
                width: 20%;
                height: 100%;
                img {
                    width: 80%;
                }
            }
            
            .navbar__menu-container {
                display: flex;
                align-items: center;
                justify-content: space-between;

                .navbar__menu {
                display: flex;

                    li {
                        margin: 0 0.9rem;

                        a {
                            color: white;

                            i {
                                font-size: 0.6rem;
                                margin-left: 0.3rem;
                                vertical-align: middle;
                            }

                            i.myArea {
                                font-size: 1rem;
                            }
                        }
                    }

                }

                .input-container {
                    display: flex;
                    justify-content: space-between;
                    align-items: center;
                    height: 40px;
                    background-color: white;
                    border-radius: 5px;
                    overflow: hidden;
                    padding: 0 8px;

                    input {
                        width: 100%;
                        height: 100%;
                        border: none;
                        outline: none;
                    }

                    .search {
                        color: #1f9efb;
                    }
                }
            }

            
        }

        
    }
</style>