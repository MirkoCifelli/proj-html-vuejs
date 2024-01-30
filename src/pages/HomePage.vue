<script>

export default {
    data() {
        return {
            imgBrand:[
                {
                    img : '../assets/brand-01.png'
                    
                },
                {
                    img : '../assets/brand-02.png'
                    
                },
                {
                    img : '../assets/brand-03.png'
                    
                },
                {
                    img : '../assets/brand-04.png'
                    
                },
                {
                    img : '../assets/brand-05.png'
                    
                }
            ],
            categoryImg:[
                {
                    img : 'category-image-02-446x550_t.jpg',
                    name:'Batman',
                    a:'Shop now'
                },
                {
                    img : 'category-image-01-446x550_t.jpg',
                    name:'Bayonetta',
                    a:'Shop now'
                },
                {
                    img : 'category-image-03-446x550_t.jpg',
                    name:'Dark Soul',
                    a:'Shop now'
                }
            ],
            mostLatestImg:[
                {
                    img : 'cms-banner-01.jpg',
                    name:'The Battelfield Naval Strike',
                    tag:'Most popular'
                },
                {
                    img : 'cms-banner-02.jpg',
                    name:'Assasin s Creed Unity Game',
                    tag:'Latest Game'
                }     
            ],
            discountImg:[
                {
                    img : 'cms-banner-03.jpg',
                    name:'Dragon s Dogma Video Game',
                    tag:'20% Discount'
                },
                {
                    img : 'cms-banner-04.jpg',
                    name:'Word Of Tanks New Game',
                    tag:'30% Discount'
                }     
            ],
            newGameBlogImg:[
                {
                    img:'/Nisi-ut-aliquid-ex-ea-com.jpg',
                    text:'Lorem ipsum 10 aggiugni qualcosa anche tu',
                    date:" Jan 18, 2001",
                    comment:' 0 comment'
                },
                {
                    img:'/Architecto-beatae-vitae-dicta.jpg',
                    text:'Lorem ipsum 10 aggiugni qualcosa anche tu a',
                    date:" May 30, 2021",
                    comment:' 0 comment'
                },
                {
                    img:'/At-vero-eos-et-accusamus.jpg',
                    text:'Lorem ipsum 10 aggiugni qualcosa anche tu b',
                    date:" April 13, 2021",
                    comment:' 0 comment'
                }
            ]
            
        };
    },
    methods:{
        getImagePath: function(imgPath){
                return new URL(imgPath, import.meta.url).href;
            },
    }
}
</script>

<template>

    <!-- jumbotron -->
    <div class="container-fluid">
        <div class="jumbotron ">
            <div id="carouselExample" class="carousel slide">
                <div class="carousel-inner">
                    <div class="carousel-item active position-relative ">
                    <img src="https://images-wixmp-ed30a86b8c4ca887773594c2.wixmp.com/f/f6c6b28e-9355-417e-b284-61503cd73b4c/deh4jpq-3c00c9da-41a9-4cac-9a0c-f28da52ff45c.png/v1/fill/w_800,h_400,q_70,strp/resident_evil_3_remake_wallpaper_by_kaelwolfgang_deh4jpq-pre.jpg?token=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJzdWIiOiJ1cm46YXBwOjdlMGQxODg5ODIyNjQzNzNhNWYwZDQxNWVhMGQyNmUwIiwiaXNzIjoidXJuOmFwcDo3ZTBkMTg4OTgyMjY0MzczYTVmMGQ0MTVlYTBkMjZlMCIsIm9iaiI6W1t7InBhdGgiOiJcL2ZcL2Y2YzZiMjhlLTkzNTUtNDE3ZS1iMjg0LTYxNTAzY2Q3M2I0Y1wvZGVoNGpwcS0zYzAwYzlkYS00MWE5LTRjYWMtOWEwYy1mMjhkYTUyZmY0NWMucG5nIiwiaGVpZ2h0IjoiPD03MjAiLCJ3aWR0aCI6Ijw9MTI4MCJ9XV0sImF1ZCI6WyJ1cm46c2VydmljZTppbWFnZS53YXRlcm1hcmsiXSwid21rIjp7InBhdGgiOiJcL3dtXC9mNmM2YjI4ZS05MzU1LTQxN2UtYjI4NC02MTUwM2NkNzNiNGNcL2thZWx3b2xmZ2FuZy00LnBuZyIsIm9wYWNpdHkiOjk1LCJwcm9wb3J0aW9ucyI6MC40NSwiZ3Jhdml0eSI6ImNlbnRlciJ9fQ.yz3PE5FNTCRVXn7Wc2beKGASR9gpi0wsOc05qkDbSrQ" class="d-block w-100" alt="...">
                    <div class="info-jumbo position-absolute text-white cordinate-absolute">
                        <h5>
                            Upcoming Stock
                        </h5>
                        <h2>
                            Resident Evil 3 Remake
                        </h2>
                        <button class="button">
                            Shop now
                        </button>
                    </div>
                    </div>
                    <div class="carousel-item position-relative">
                    <img src="https://static.bandainamcoent.eu/high/jump-force/jump-force/00-page-setup/jump-force_game-thumbnail2.jpg" class="d-block w-100 jumbo-img" alt="...">
                    <div class="info-jumbo position-absolute text-white cordinate-absolute">
                        <h5>
                            Upcoming Stock
                        </h5>
                        <h2>
                            New jump-force Goku
                        </h2>
                        <button class="button">
                            Shop now
                        </button>
                    </div>
                    </div>
                    
                </div>
                <button class="carousel-control-prev" type="button" data-bs-target="#carouselExample" data-bs-slide="prev">
                    <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                    <span class="visually-hidden">Previous</span>
                </button>
                <button class="carousel-control-next" type="button" data-bs-target="#carouselExample" data-bs-slide="next">
                    <span class="carousel-control-next-icon" aria-hidden="true"></span>
                    <span class="visually-hidden">Next</span>
                </button>
            </div>
        </div>
    </div>

    <!-- Most e latest  -->
    <div class="container p-2 ">
        <div class="row">
            <div class="col-12">
                <div class=" d-flex justify-content-around  p-5 ">
                    <div class="d-flex align-items-center hover-effect">
                        <i class="fa-solid fa-truck fs-1"></i>
                        <div class="ms-3">
                            <h6>Free Delivery</h6>
                            <span>Free Shipping on All Order</span>
                        </div>
                    </div>

                    <div class=" d-flex align-items-center hover-effect">
                        <i class="fa-solid fa-percent fs-1 "></i>
                        <div class="ms-3">
                            <h6>Money Return</h6>
                            <span>Back Guarantee in 7 days</span>
                        </div>
                    </div>

                    <div class=" d-flex align-items-center hover-effect">
                        <i class="fa-solid fa-sack-dollar fs-1 "></i>
                        <div class="ms-3">
                            <h6>Member Discount</h6>
                            <span>On every order over $130.00</span>
                        </div>
                    </div>

                    <div class=" d-flex align-items-center hover-effect">
                        <i class="fa-solid fa-hand-holding-dollar fs-1 "></i>
                        <div class="ms-3">
                            <h6>Return Policy</h6>
                            <span>Support 24 hour a day</span>
                        </div>
                    </div>
    
                   
                </div>
            </div>
            <div class="col-6" v-for="(cms,i) in mostLatestImg" :key="i">
                <div class="img-most position-relative ">
                    <img :src="getImagePath('../assets/'+ cms.img)" alt="">
                    <div class="img-most-info">
                        <h5>
                            {{cms.tag}}
                        </h5>
                        <h6>
                            {{cms.name}}
                        </h6>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <!-- special category -->
    <div class="container">
        <div class="row">
            <div class="col-12 mb-4">
                <h2 class="text-center pt-3 ">
                    Special<span> Cat</span>egory
                </h2>
            </div>
            <div class="col-4" v-for="(category,i) in categoryImg" :key="i">
                <div class="card">
                    <img :src="getImagePath('../assets/'+ category.img)" alt="">
                    <div class="special-category-info ">
                        <div class="card-div">
                            {{ category.name}}
                        </div>
                        <div class="shop-now">
                            <a href="#">{{ category.a }}</a>
                         </div>
                    </div>
                </div>
            </div>
            
        </div>
    </div>

    <!-- OurProducts -->
    <div class="container">
        <div class="row pb-4 ">
            <div class="col-12 mb-4">
                <h2 class="text-center pt-3 ">
                    Our P<span>ro</span>ducts
                </h2>
            </div>
            <div class="col-12 mb-3">
                <nav>
                    <ul>
                        <li>
                            Featured
                        </li>
                        <li>
                            New Arrival
                        </li>
                        <li>
                            Best Seller
                        </li>
                    </ul>
                </nav>
            </div>
            <div class="col-3">
                <div class="card">
                    <img src="../assets/04.jpg" alt="">
                    <div class="special-category-info ">
                        <div class="card-div">
                            Batman
                        </div>
                        
                    </div>
                </div>
            </div>
            <div class="col-3">
                <div class="card">
                    <img src="../assets/09.jpg" alt="">
                    <div class="special-category-info ">
                        <div class="card-div">
                            Batman
                        </div>
                        
                    </div>
                </div>
            </div>
            <div class="col-3">
                <div class="card">
                    <img src="../assets/03.jpg" alt="">
                    <div class="special-category-info ">
                        <div class="card-div">
                            Batman
                        </div>
                        
                    </div>
                </div>
            </div>
            <div class="col-3">
                <div class="card">
                    <img src="../assets/11.jpg" alt="">
                    <div class="special-category-info ">
                        <div class="card-div">
                            Batman
                        </div>

                    </div>
                </div>
            </div>
        </div>

        <div class="row">
            <div class="col-6" v-for="(discount,i) in discountImg" :key="i">
                <div class="img-most position-relative ">
                    <img :src="getImagePath('../assets/'+ discount.img)" alt="">
                    <div class="img-most-info">
                        <h5>
                            {{discount.tag}}
                        </h5>
                        <h6>
                            {{discount.name}}
                        </h6>
                    </div>
                </div>
            </div>
        </div>

    </div>

    <!-- Deal Of the Day -->
    <div class="container">
        <div class="row  pb-4 ">
            <div class="col-12 p-4">
                <h2 class="text-center pt-3 ">
                    Deal Of<span> Th</span>e Day
                </h2>
            </div>

            <div class="col-12 mb-3">
                <nav>
                    <ul>
                        <li>
                            Day
                        </li>
                        <li>
                            hours
                        </li>
                        <li>
                            min
                        </li>
                        <li>
                            sec
                        </li>
                    </ul>
                </nav>
            </div>

            <div class="col-3">
                <div class="card">
                    <img src="../assets/04.jpg" alt="">
                    <div class="special-category-info ">
                        <div class="card-div">
                            Batman
                        </div>
                        
                    </div>
                </div>
            </div>
            <div class="col-3">
                <div class="card">
                    <img src="../assets/04.jpg" alt="">
                    <div class="special-category-info ">
                        <div class="card-div">
                            Batman
                        </div>
                        
                    </div>
                </div>
            </div>
            <div class="col-3">
                <div class="card">
                    <img src="../assets/04.jpg" alt="">
                    <div class="special-category-info ">
                        <div class="card-div">
                            Batman
                        </div>
                        
                    </div>
                </div>
            </div>
            <div class="col-3">
                <div class="card">
                    <img src="../assets/04.jpg" alt="">
                    <div class="special-category-info ">
                        <div class="card-div">
                            Batman
                        </div>
                        
                    </div>
                </div>
            </div>

        </div>
    </div>

    <!-- Staff -->
    <div class="container-fluid pb-3 ">
        <div class="img-container-staff">
            <!-- <img src="../assets/parallax.jpg" alt=""> -->
            <div class="container d-flex flex-wrap justify-content-center p-5">
                <div class="img-staff position-relative">
                    <img src="../assets/t5-1-100x100_left.jpg" alt="">
                </div>
                <div class="absolute-quote">
                    <img src="../assets/quote.png" alt="">
                </div>
                <div class="staff-info d-flex flex-wrap align-items-center justify-content-center">
                    <h4 class=" m-1">Lules Charls</h4><span>(Web designer)</span>
                    <p>
                        Lorem ipsum dolor sit, amet consectetur adipisicing elit. Labore harum iste ratione fuga adipisci repudiandae aut aperiam quae dolor explicabo omnis, recusandae vel totam quasi? Nemo rem laborum aperiam unde!
                    </p>
                </div>
                <div class=" text-center">
                    <span class="dot"></span>
                    <span class="dot"></span>
                    <span class="dot"></span>
                </div>
            </div>
        </div>
    </div>
    <!-- New game blogs -->
    <div class="container">
        <div class="row">
            <div class="col-12 p-4">
                <h2 class="text-center pt-3 ">
                    New G<span>ame</span> Blogs
                </h2>
            </div>
            <div class="col-12">
                <div id="carouselExample" class="carousel slide">
                    <div class="carousel-inner">
                        <div class="carousel-item active">
                            <div class="card-wrapper d-flex justify-content-evenly">
                                <div class="card" style="width: 18rem;" v-for="(blog,i) in newGameBlogImg" :key="i">
                                    <img :src="getImagePath('../assets/'+ blog.img)" class="card-img-top" alt="...">
                                    <div class="card-body cardinfoblog">
                                        <div class="co-orange d-flex">
                                            <i class="fa-regular fa-calendar-days">{{blog.date}}</i><i class="fa-solid fa-comment ms-2">{{blog.comment}}</i>
                                        </div>
                                        <p class="card-text">{{blog.text}}</p>
                                    </div>
                                </div> 
                            </div>
                        </div>
                        <div class="carousel-item">
                            <div class="card-wrapper">
                                <div class="card" style="width: 18rem;">
                                    <img src="..." class="card-img-top" alt="...">
                                    <div class="card-body">
                                        <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="carousel-item">
                            <div class="card-wrapper">
                                <div class="card" style="width: 18rem;">
                                    <img src="..." class="card-img-top" alt="...">
                                    <div class="card-body ">
                                        <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    <button class="carousel-control-prev" type="button" data-bs-target="#carouselExample" data-bs-slide="prev">
                        <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                        <span class="visually-hidden">Previous</span>
                    </button>
                    <button class="carousel-control-next" type="button" data-bs-target="#carouselExample" data-bs-slide="next">
                        <span class="carousel-control-next-icon" aria-hidden="true"></span>
                        <span class="visually-hidden">Next</span>
                    </button>
                    </div>
            </div>

            <hr>
            <div class="contenitore-5 d-flex justify-content-evenly mb-5">
                
                <div class="contenitore-brand" v-for="(brand,i) in imgBrand" :key="i">
                    <img :src="getImagePath('../assets/'+ brand.img)" alt="">
                </div>

            </div>
        </div>
    </div>

</template>

<style lang="scss" scoped>
.container-fluid{
    padding: 0%;
    .jumbotron{
    .cordinate-absolute{
    top: 30%;
    left: 20%;
    }
    h5{
        color: black;
        background-color: #F9AA01;
        width: 40%;
        text-align: center;
        clip-path: polygon(6% 1%, 100% 0%, 96% 100%, 0% 100%);
        padding: 5px;
        font-weight: bold;
    
    }
    h2{
        width: 70%;
        margin-top: 20px;
        word-wrap: break-word;
        font-size: 3em;
    }
    .button {
        background-color: #ffffff; /* Green */
        border: none;
        color: black;
        padding: 10px 20px;
        text-align: center;
        text-decoration: none;
        display: inline-block;
        font-size: 14px;
        font-weight: bold;
        margin-top: 40px;
        &:hover{
            color: black;
            background-color: #F9AA01;
        }
}
}
}
.container{
    color: #ffffff;
    .hover-effect{
        &:hover{
            color: #F9AA01;
        }
    }
    img{
        width: 100%;
        height: 100%;
    }
    .img-most-info{
        position: absolute;
        top: 30%;
        right: 5%;
    }
    h6{
        font-size: 20px;
        word-wrap: break-word;
        
    }
    h5{
        color: black;
        background-color: #F9AA01;
        width: 60%;
        text-align: center;
        clip-path: polygon(6% 1%, 100% 0%, 96% 100%, 0% 100%);
        padding: 5px;
        font-weight: bold;
        margin-bottom: 20px;
    }
    h2{
        span{
            border-bottom: 2px solid #F9AA01;
            font-size: 30px;
            padding-bottom: 10px;
        
        }
    }
    span{
        font-size: 12px;
    }
    .card{
        position: relative;
        border: 0;
        .special-category-info{
            width: 100%;
            height: 20%;
            position: absolute;
            bottom: 0%;
            left: 0;
            background-color: #1D1427;
            opacity: 0.5;
            padding: 20px;
            &:hover{
                opacity: 0.95;
            }
            .card-div{
                color: #ffffff;
                font-weight: bold;
                
            }
            .shop-now
                a{
                color: #F9AA01;

            }
        }
    }
    nav{
        ul{
            list-style: none;
            display: flex;
            align-items: center;
            justify-content: center;
        }
        li{
            padding: 10px 40px;
            border: 1px solid rgb(66, 66, 66);
        }
    }
}
.container-fluid{
    .img-container-staff{
        width: 100%;
        height: 300px;
        background-image: url(../assets/parallax.jpg);
        background-repeat: no-repeat;
        background-position: center;
        .container{
            .img-staff{
                width: 100px;
                height: 100px;
                img{
                    width: 100%;
                    height: 100%;
                    border-radius: 50%;
                    border: 1px solid #F9AA01;
                }
            }
            .absolute-quote{
                position: absolute;
                left: 46%;
                background-color: #F9AA01;
                height: 20px;
                width: 20px;
                border-radius: 50%;
                line-height: 1;
               
            }
            .staff-info{
                margin: 10px 20px;
                h4{
                    font-size: 20px;
                }
                span{
                    font-size: 20px;
                    color: #F9AA01;
                    margin-left: 4px;
                }
            }
            .dot {
                height: 10px;
                width: 10px;
                background-color: #bbb;
                border-radius: 50%;
                display: inline-block;
                margin-left: 5px;
                &:first-of-type{
                    background-color: #F9AA01;
                }
            }
        }
    }
}
.container-5{
    .contenitore-brand{
        width: 50px;
        height: 50px;
        img{
            width: 100%;
            height: 100%;
        }
    }
}
 
.cardinfoblog{
    background-color: #1D1427;
    color: white
    
}
.co-orange{
    color: #F9AA01;
}

    

</style>