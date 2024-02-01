<script>
export default {
    data() {
        return {
            codezeel:[
                {
                    iconClass:"fa-solid fa-globe fa-2xl i-style",
                    label:"Easy to use",
                    description:"We’ve put a lot of thought in giving you the best possible experience to make your job easier.",
                },
                {
                    iconClass:"fa-solid fa-comments fa-2xl",
                    label:"Outstanding Support",
                    description:"Modules comes fully documented with step by step instructions. access premium support forum.",
                },
                {
                    iconClass:"fa-regular fa-heart fa-2xl",
                    label: "Simply Beautiful",
                    description:"Our themes are not just nicely coded, they are built to show your visitors how much you care for beauty and for design.",
                },
                {
                    iconClass:"fa-solid fa-cube fa-2xl",
                    label:"Careful Crafted",
                    description:"Coded with WordPress best practices in mind, Modules will give you an amazing looking site easier.",
                },
                {
                    iconClass:"fa-solid fa-table-cells fa-2xl",
                    label:"20+ Bulilder Module",
                    description:"Create as many modules as you want. Personalize them and build with them your pages.",
                },
                {
                    iconClass:"fa-regular fa-circle-play fa-2xl",
                    label:"WP Video Training",
                    description:"Enjoy a comprehensive collection of WordPress 101 video tutorials on our membership training area.",
                },
            ],
            socialIconTeamMember: [
                'fa-brands fa-facebook fa-beat-fade fa-xl',
                'fa-brands fa-twitter fa-beat-fade fa-xl',
                'fa-brands fa-youtube fa-beat-fade fa-xl',
                'fa-brands fa-linkedin fa-beat-fade fa-xl'
            ],

            chooseUs: [
            {
                titleH4 : 'Why choose us?',
                textParagraph : 'Nullam dictum felis eu pede mollis pretium. Integer tincidunt. Cras dapibus. Vivamus elementum semper nisi. Aenean vulputate eleifend tellus. Aenean leo ligula, porttitor eu, consequat vitae, eleifend ac, enim. Quisque rutrum. Aenean imperdiet. Etiam ultricies nisi vel augue.consequat vitae, eleifend ac, enim. Quisque rutrum. Aenean imperdiet.'
            }
            ],

            whyChoose: [
            {
                textParagraph : 'Praesent sed ex vel mauris ele.',
            },
            {
                textParagraph : 'Nam vel luctus nulla, eget interdum metus',
            },
            {
                textParagraph : 'Temporibus autem',
            },
            {
                textParagraph : 'Excepteur sint occaecat'
            }
            ],

            teamMember: [
            {
                image: "https://capricathemes.com/wordpress/WCM04/WCM040086/wp-content/uploads/2019/06/s2-2-1-600x600_t.jpg",
                nameStaff: 'Monic Marty',
                role: '(Assistent)',
                occupation: 'Lorem ipsum, dolor sit amet consectetur adipisicing elit. Sed, dolor sit vel....',
            },
            {
                image: "https://capricathemes.com/wordpress/WCM04/WCM040086/wp-content/uploads/2019/06/s1-2-1-600x600_t.jpg",
                nameStaff: 'Nemo Enim',
                role: '(Manager)',
                occupation: 'Lorem ipsum, dolor sit amet consectetur adipisicing elit. Sed, dolor sit vel....',
            },
            {
                image: "https://capricathemes.com/wordpress/WCM04/WCM040086/wp-content/uploads/2019/06/s4-2-1-600x600_t.jpg",
                nameStaff: 'Vilorano Jeo',
                role: '(Designer)',
                occupation: 'Lorem ipsum, dolor sit amet consectetur adipisicing elit. Sed, dolor sit vel....',
            },
            {
                image: "https://capricathemes.com/wordpress/WCM04/WCM040086/wp-content/uploads/2019/06/s5-2-1-600x600_t.jpg",
                nameStaff: 'Mark Marley',
                role: '(CEO)',
                occupation: 'Lorem ipsum, dolor sit amet consectetur adipisicing elit. Sed, dolor sit vel....',
            },
            {
                image: "https://capricathemes.com/wordpress/WCM04/WCM040086/wp-content/uploads/2019/06/s4-2-1-600x600_t.jpg",
                nameStaff: 'Lili Anderson',
                role: '(Manager)',
                occupation: 'Lorem ipsum, dolor sit amet consectetur adipisicing elit. Sed, dolor sit vel....',
            },
            ],

            imgBrand:[
                {
                    img : 'brand-01.png'
                    
                },
                {
                    img : 'brand-02.png'
                    
                },
                {
                    img : 'brand-03.png'
                    
                },
                {
                    img : 'brand-04.png'
                    
                },
                {
                    img : 'brand-05.png'
                    
                }
            ],

            counter: [
            {
                numberStats: '50',
                textStats: 'Hours Per Week'
            },
            {
                numberStats: '20.052',
                textStats: 'Line Of Code'
            },
            {
                numberStats: '980',
                textStats: 'Projects Completed'
            },
            {
                numberStats: '334',
                textStats: 'Shots On Dribble'
            },
            
            ]
        };
    },

    methods : {
        getImagePath: function(imgPath){
                return new URL(imgPath, import.meta.url).href;
            },
    }
}
</script>

<template>
        <div class="background-aboutPage">
            <!--PRIMA SEZIONE-->
            <div class="container">
                <div class="d-flex fs-6 align-items-center ">
                    <a class="text-decoration-none text-white" href="#">Home &nbsp;</a> >>
                    <div class="fs-6 ms-2">
                        About Us
                    </div>
                </div>

                <div class="fs-4 ">
                    About Us
                </div>
            </div>

            <!--SECONDA SEZIONE-->           
            <div class="container mt-4">
                <div class="row my-margin">
                    <div class="col-12 d-flex justify-content-between mb-4">
                        <div class="d-flex fs-6 align-items-center">
                    <a class="text-decoration-none text-white" href="#">Home &nbsp;</a> >>
                    <div class="fs-6 ms-2">
                        About Us
                    </div>
                </div>

                <div class="fs-4 ">
                    About Us
                </div>
                    </div>
                    <div class="col-6">
                        <div id="carouselExampleInterval" class="carousel slide" data-bs-ride="carousel">
                            <div class="carousel-inner">
                                <div class="carousel-item active" data-bs-interval="10000">
                                    <img src="../assets/Blandit-praesen-volupta.jpg" class="d-block w-100" alt="...">
                                </div>
                                <div class="carousel-item" data-bs-interval="2000">
                                    <img src="../assets/Et-quasi-architecto-beate.jpg" class="d-block w-100" alt="...">
                                </div>
                                <div class="carousel-item">
                                    <img src="../assets/Laborum-et-dolor-fuga-Et.jpg" class="d-block w-100" alt="...">
                                </div>
                            </div>
                            <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleInterval" data-bs-slide="prev">
                                <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                                <span class="visually-hidden">Previous</span>
                            </button>
                            <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleInterval" data-bs-slide="next">
                                <span class="carousel-control-next-icon" aria-hidden="true"></span>
                                <span class="visually-hidden">Next</span>
                            </button>
                        </div>
                    </div>

                    <div v-for="(elem, i) in chooseUs" :key="i" class="col-6">
                        <h4>
                            {{ elem.titleH4 }}
                        </h4>
                        <div class="shortbar"></div>
                        <p>
                            {{ elem.textParagraph }}
                        </p>
                        <ul class="list-unstyled ">
                            <li v-for="(choose, i) in whyChoose " :key="i">
                                <i class="fa-solid fa-circle fa-xs" style="color: rgb(250, 171, 0);"></i>
                                <a class="m-2" href="#">{{ choose.textParagraph }}</a>
                            </li>
                        </ul>
                        <button class="p-2 mt-2 mb-5 button-talk">
                            Let's Talk
                        </button>
                    </div>
                </div>
            </div>

            <!--TERZA SEZIONE-->
            <div class="container-2">
                <h3 class="text-white">
                    Codezeel History
                </h3>
                <div class="shortbar-section-two"></div>

                <div class="row text-white d-flex text-center ">
                    <!-- oarte nuova -->
                    <div class="col-4 mb-4 d-flex flex-column align-items-center" v-for="(elem, i) in codezeel" :key="i">
                        <div class="background-orange">
                            <i :class="elem.iconClass"></i>
                        </div>
                        <div>
                            <h5 class="mt-3">
                                {{ elem.label }}
                            </h5>
                        </div>
                        <div>
                            <p>
                                {{ elem.description }}
                            </p>
                        </div>
                    </div>
                </div>
            </div>

            <!--QUARTA SEZIONE-->
            <div class="container-2 mt-5 position-relative ">
                <div class="sfondo">
                    <div class="row">
                        <div v-for="(counters, i) in counter" :key="i" class="col-3 text-center padding-counter">
                            <div class="fs-1 text-white text-center  mt-3 mb-3">{{ counters.numberStats }}</div>
                            
                                <p class="ps-4">{{ counters.textStats }}</p>
                            
                        </div>
                    </div>
                </div>
            </div>

            <!--QUINTA SEZIONE-->
            <div class="container-2">
                <h3 class="text-white">
                    Our Team Member
                </h3>
                <p class="text-center text-white ">
                    Meet the many faces that help power the Elegant Themes community
                </p>
                <div class="shortbar-section-two"></div>
                <div class="row text-white carousel_container">
                    <div v-for="(member, i) in teamMember" :key="i" class="col-3">
                        <div class="w-100 position-relative ">
                            <ul class="list-unstyled text-black position-absolute ul-icon-team-member ">
                                <li v-for="(socialIcon, i) in socialIconTeamMember" :key="i" class="ul-icon-team-member mt-2 p-1">
                                    <i :class="socialIcon" class="orange-li"></i>
                                </li>
                            </ul>
                            <img class="mb-2 w-100 " :src="member.image" alt="">
                        </div>
                        <div>
                            <a href="#"><strong class="fs-5 me-2"> {{ member.nameStaff }}</strong></a>
                            <span class="fst-italic"> {{ member.role }}</span>
                        </div>
                        <div>
                            <p class="mt-2">
                                {{ member.occupation }}
                            </p>
                        </div>
                    </div>
                </div>
            </div>

            <!--SESTA SEZIONE-->
            <div class="contenitore-5 d-flex justify-content-evenly mt-5 p-5">
                
                <div class="contenitore-brand" v-for="(brand,i) in imgBrand" :key="i">
                    <img :src="getImagePath('../assets/'+ brand.img)" alt="">
                </div>

            </div>
        </div>
</template>

<style lang="scss" scoped>


//SECTION 1
.background-aboutPage{
    background-image: url('../assets/body-bg.jpg');

    .container{
        color: white;
        display: flex;
        justify-content: space-between;
        align-items: center;
        width: 90%;
        margin: auto;
    }

    .my-margin{
        margin-top: 100px;
    }

    .shortbar{
        border-bottom: 2px solid #f9aa01;
        width: 54px;
        margin-top: 20px;
        margin-bottom: 20px;
    }

    p, a{
        color: rgb(135, 135, 135);
        font-size: 14px;
    }

    ul > li*{
        margin-top: 10px;
    }

    a{
        text-decoration: none;
    }

    a:hover{
        color: rgb(250, 171, 0);
    }

    .button-talk{
        width: 20%;
        background-color: rgb(34, 22, 46);
        color: white;
        border: 0px;

        &:hover{
            color: rgb(250, 171, 0);
        }

    }
}


//SECTION 2
.container-2{
    width: 90%;
    margin: auto;

    h3{
        margin-top: 80px;
        text-align: center;
    }

    .shortbar-section-two{
        border-bottom: 2px solid #f9aa01;
        width: 54px;
        margin: 0 auto;
        margin-top: 15px;
        margin-bottom: 25px;
        }

        .background-orange{
        background-color: orange;
        width: 70px;
        height: 70px;
        border-radius: 50%;
        line-height: 4.2;
        transition: 0.5s;
        }

        .background-orange:hover{
            width: 80px;
            height: 80px;
            line-height: 4.7;
        }

        p{
            margin-right: 30px;
        }
}


//SECTION 3

.container-2{

    .carousel_container{
    width: 100%;
    flex-wrap: nowrap;
    overflow: auto;
    
    >*{
        flex-shrink: 0;
    }
}

    .position-icon-card-member{
        position: absolute;
        top: 15px;
    }

    
}

//SECTION 4
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

.sfondo{
    width: 100%;
    height: 200px;
    background-color:rgb(23, 15, 31);
    margin: auto;

    .padding-counter{
        padding: 30px 0;
    }

    p{
        color: rgb(135, 135, 135);
    }
}
// SECTION 5
.w-100{
    ul{
    opacity: 0;
    &.ul-icon-team-member:hover{
        
        opacity: 1;

    }
    .orange-li:hover{
        color: rgb(250, 171, 0);
    }
}
}



</style>