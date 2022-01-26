<template>
    <nav>
        <div class="logo">
            <img src="../assets/images/light-logo.png" alt="">
        </div>
        <div class="navbar__menu-container">
            <ul class="navbar__menu">
                <li
                  v-for="(link, index) in navLink"
                  :key="index"
                ><a :href="link.src">{{link.label}}<i class="fas fa-chevron-down"></i></a></li>
                <li>
                    <a href="#"><i class="fas fa-shopping-cart myArea"></i></a>
                    <div class="cart-items">
                        <span>0</span>
                    </div>
                </li>
                <li><a href="#"><i class="far fa-user-circle myArea"></i></a></li>
            </ul>

            <div class="input-container">
                <input placeholder="Search..." type="text">
                <i class="fas fa-search search"></i>
            </div>
        </div>
    </nav>
</template>

<script>
export default {
    name: "NavBar",
    data() {
        return {
            navLink: [
                {
                    label: "Home",
                    src: "#"
                },
                {
                    label: "Pages",
                    src: "#"
                },
                {
                    label: "Courses",
                    src: "#"
                },
                {
                    label: "Features",
                    src: "#"
                },
                {
                    label: "Blog",
                    src: "#"
                },
                {
                    label: "Shop",
                    src: "#"
                },
            ] 
            
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../assets/scss/partials/_variables.scss";

    nav {
        display: flex;
        justify-content: space-between;
        width: 100%;
        height: 80px;
        padding: 1rem;

        .logo {
            display: flex;
            align-items: center;
            width: 20%;
            height: 100%;

            img {
                width: 70%;
            }
        }
        
        .navbar__menu-container {
            display: flex;
            align-items: center;
            justify-content: space-between;

            .navbar__menu {
                display: flex;

                li {
                    position: relative;
                    margin: 0 0.6rem;

                    .cart-items {
                        position: absolute;
                        top: -5px;
                        right: -8px;
                        display: flex;
                        justify-content: center;
                        align-items: center;
                        width: 15px;
                        height: 15px;
                        border: 1px solid $portGore;
                        border-radius: 50%;
                        background-color: white;
                        color: black;

                        span {
                            font-size: 0.6rem;
                            line-height: 15px;
                            font-weight: 600;
                        }
                    }

                    a {
                        color: white;

                        &:hover {
                            text-decoration: underline;
                        }

                        i {
                            margin-left: 0.3rem;
                            vertical-align: middle;
                            font-size: 0.5rem;
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
                padding: 0 8px;
                border-radius: 5px;
                background-color: white;
                overflow: hidden;

                input {
                    width: 100%;
                    height: 100%;
                    border: none;
                    outline: none;
                }

                .search {
                    color: $dodgerBlue;
                }
            }
        }
    }

</style>