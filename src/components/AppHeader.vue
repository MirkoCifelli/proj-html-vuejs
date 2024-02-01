<script>
export default {
    data() {
        return {
           
            navMenu: [
                'Home',
                'Shop',
                'Blog',
                'Media',
                'ShortCode',
            ],

            needHelp: [
                '0000-000-00',
                '9876543210',
                '9876-543-210',
                '+9876543210',
            ],

            features: [
                'FAQ Page',
                'Typhography',
                'Sitemap',
            ]
        };
    },
    methods: {

    }
}
</script>

<template>
    <header>

        <!--PRIMA SEZIONE HEADER-->
        <div class="background-header">
            <div class="container">
                <div class="d-flex">
                    <a class="text-color-wishlist" href="#">Wishlist(0)</a>
                    <div class="ms-3">
                        <button class="dropdown-toggle text-color-wishlist background-features" data-bs-toggle="dropdown">
                            Need Help ?
                        </button>
                        <ul class="dropdown-menu color-text-features background-menu">
                            <li v-for="(help, i) in needHelp" :key="i">
                                 <a class="dropdown-item character-special font-size-need-help" href="#"> &#128222;	{{help}}</a>
                            </li>
                            </ul>
                    </div>
                </div>

                <div class="d-flex ms-5 hover-call-number">
                    CALL 24/7.
                    <div class="ms-3">
                        800-8754-987
                    </div>
                </div>
            </div>
        </div>
        <div class="line-header"></div>


        <!--SECONDA SEZIONE HEADER-->
        <aside>
            <div class="background-header">
                <div class="container text-white">
                    <div>
                        <img class="header-logo" src="../assets/logo.png" alt="">
                    </div>

                    <nav>
                        <ul class="d-flex p-0 m-0">
                            <li v-for="(elem, i) in navMenu" :key="i">
                                <router-link :to="{name: 'home'}">
                                <a href="#"> {{ elem }}</a>
                                </router-link>
                            </li>
  
                            <li>
                                <div class="dropdown">
                                    <button class="dropdown-toggle background-features text-white" data-bs-toggle="dropdown">
                                        Features
                                    </button>
                                    <ul class="dropdown-menu hover-feat color-text-features background-menu">
                                        <li v-for="(feature, i) in features" :key="i">
                                            <a class="dropdown-item" href="#">
                                                {{ feature }}
                                            </a>
                                        </li>
                                        
                                        <li>
                                            <router-link :to="{name: 'about'}">
                                                <a class="dropdown-item character-special" href="#">
                                                    About Us
                                                </a>
                                            </router-link>
                                        </li>
                                        
                                        <li>
                                            <router-link :to="{name: 'contact'}">
                                                <a class="dropdown-item character-special" href="#"> 
                                                    Contact Us
                                                </a>
                                            </router-link>
                                        </li>
                                    </ul>
                                </div>
                            </li>
                        </ul>
                    </nav>

                    <div class="d-flex">
                        <div>
                            <a href="#">
                                <i class="fa-solid fa-magnifying-glass" style="color: #ffffff;"></i>
                            </a>
                        </div>
                        <div>
                            <a href="">
                                <i class="fa-regular fa-user" style="color: #ffffff;"></i>
                            </a>
                        </div>
                        <div>
                            <a href="#">
                                <i class="fa-solid fa-bag-shopping" style="color: #ffffff;"></i>
                                (0) £0.00
                            </a>
                        </div>
                    </div>
                </div>
            </div>
                <div class="line-header"></div>
        </aside>
    </header>
</template>

<style lang="scss" scoped>

header{
    width: 100%;
    position: fixed;
    z-index: 5;

    .background-header{ 
        background-image: url('../assets/body-bg.jpg');
    }
    .container{
        width: 90%;
        color: rgb(166, 166, 166);
        margin: auto;
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 15px;
    }

        .header-logo{
            margin-right: 20px;
            height: 35px;
            width: 170px;
        }

            .background-menu{
                background-color: rgb(28, 20, 38);
            }

            .font-size-need-help{
                font-size: 12px;
            }

            & ul > li{
                margin-left: 20px;
                margin-right: 20px;
                list-style: none;
            }

            a{
                text-decoration: none;
                color: white;
            }

            a:hover{
                color: rgb(250, 171, 0);
            }

            .text-color-wishlist{
                color: rgb(166, 166, 166);
            }

            & div *i{
                margin-left: 10px;
            }

            .dropdown > ul > li > a{
                color: rgb(135, 135, 135);

                &:hover{
                    color: rgb(250, 171, 0);
                }
            }

            .character-special{
                color: rgb(135, 135, 135);

                & :hover, .hover-call-number:hover{
                    color: rgb(250, 171, 0);
                }
            }

            .hover-call-number:hover {
                color: rgb(250, 171, 0);
            }

            .background-features{
                background-color: rgb(28, 20, 38);
                border: 0px;
                &:hover{
                    color: rgb(250, 171, 0) !important;
                }
            }
            
    }


.line-header{
            background-color: rgb(52, 44, 61);
            height: 1px;
        }

</style>