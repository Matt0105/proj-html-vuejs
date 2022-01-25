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

    nav {
        display: flex;
        width: 100%;
        height: 80px;
        justify-content: space-between;
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
                        background-color: white;
                        color: black;
                        height: 15px;
                        width: 15px;
                        border-radius: 50%;
                        border: 1px solid #1f2154;

                        span {
                            font-size: 0.6rem;
                            line-height: 15px;
                            font-weight: 600;
                        }
                    }

                    a {
                        color: white;

                        i {
                            font-size: 0.5rem;
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

</style>