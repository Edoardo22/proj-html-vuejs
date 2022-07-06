<template lang="">
    <div class="jumbo-bg container-fluid d-flex justify-content-center">
        <div class="row container pt-5  position-relative">
            <div class="col-5">
                <div>
                    <img src="img/author-logo-round-200x205.png" alt="logo" class="img-fluid top-logo">
                </div>
                <div class="text-warning pb-4 allura">Damon Vaugh</div>
              <div v-if="index==1" class="text-white fs-1 pb-4">Best-selling author and the most influential public intellectual in the western world right now.</div>  
              <div v-if="index==1" class="text-light fs-4">- The New York Times</div>
              <div v-if="index==2" class="text-white fs-1 pb-4">Ma guarda che transizione ho fatto mattia, bella vero? </div>  
              <div v-if="index==2" class="text-light fs-4">- The junior developer scarso</div>
              <div class="text-white pt-5">
             <span @click="prev"  class="square-arrow me-2 p-3 rounded"><i class="fa-solid fa-arrow-left"></i></span>
             <span @click="next" class="square-arrow p-3 rounded"><i class="fa-solid fa-arrow-right"></i></span>
             </div>
                </div>
             <div class="col-7 d-flex ">
                <ul class="navbar-nav me-auto mb-2 mb-lg-0 NavP" v-for="(item,i) in NavList"  :key="i">
            <li>
                <a class="nav-item text-decoration-none testo-bianco px-2" v-bind:class="{'text-warning border-top border-5 pt-5 border-warning': item.active}"  @click="currentPage" :href="item.url">{{item.name}}</a>    
                   <span :class="item.class" class="icons testo-bianco"></span>
            </li>
           
            </ul>
          
             <div class="demon-pri">
                <a href="" class="text-decoration-none text-black">
                 <div class="square mb-4 text-center">
                    <img src="img/Senza_titolo-1.png" alt="" class="w-50 pt-2">
                    <div>Demos</div>
                 </div>
                 </a>
                 <a href="" class="text-decoration-none text-black">
                  <div class="square mt-4 text-center">
                    <span class="align-top text-success">$</span>
                    <span class="fs-2 text-success">39</span>
                    <div class="">On Sale</div>
                  </div>
                  </a>
            </div>
            <div class="book-pub">
                <div class="d-flex">
                    <div class=" d-flex justify-content-center pt-5 ps-5">
                        <img src="img/book-widget.png">
                    </div>
                    <div class=" pt-5 pe-0">
                        <div class=" fs-4 pb-3">LASTEST BOOK RELEASE</div>
                        <div class="text-warning pb-3">D. VAUGHN AUTOBIOGRAPHY</div>
                          <div class="">Best-selling author and the most influential public intellectual in the western world right now.</div>
                    </div>
                </div>
                <div class="d-flex text-center justify-content-center">
                    <button type="button" class="btn border-success px-5 py-2 d-flex align-items-end bg-lightGreen"> <img src="img/amazon_icon.png" class="icon-shop me-2"> Buy on Amazon</button>
                    <button type="button" class="btn border-success px-5 py-2 d-flex  align-items-end bg-lightGreen"><img src="img/Apple_logo_black.svg.png" class="icon-shop me-2">  Buy on App Store</button>
                </div>
            </div>
            </div>
             
             </div>
        </div>
    
</template>
<script>
export default {

    data() {
        return {
            NavList: [
                {
                    name: 'Home',
                    url: '#',
                    active: true,

                },
                {
                    name: 'About Me',
                    url: '#',
                    active: false,
                },
                {
                    name: 'Testimonials',
                    url: '/Testimonials',
                    active: false,
                },
                {
                    name: 'My Blog',
                    url: '/Blog',
                    active: false,
                },
                {
                    name: 'Meetups',
                    url: '/Meetups',
                    active: false,
                },
                {
                    name: 'Shop',
                    url: '/Shop',
                    active: false,
                },
                {
                    name: 'Contact Me',
                    url: '/Contact',
                    active: false,
                },
                {
                    class: 'fa-solid fa-cart-shopping',
                    active: false,
                }
            ],
            index: 1,
        }

    },
    methods: {
        currentPage() {
            this.NavList.active = true;
        },
        prev() {
            if (this.index > 1) {
                this.index--;
            }

        },
        next() {
            if (this.index <= 1) {
                this.index++;
            }
        }
    }

}
</script>


<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Allura&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap');

body {
    font-family: 'Roboto', sans-serif !important;
}

.icons:hover {
    cursor: pointer;
    transform: scale(1.5);
    transition: all 0.2s ease-in-out;
}

.text-off {
    color: rgba(255, 255, 255, 0.781) !important;
}

.icon-shop {
    width: 20px;
}

.testo-bianco {
    color: #fff;
}

.testo-bianco:hover {
    color: rgb(255, 193, 7);
}

.allura {
    font-family: 'Allura', cursive;
    font-size: 70px;
}

.jumbo-bg {
    background-image: url("../../public/img/hero-07-2x.jpg");
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
    height: 800px;
}

.square-arrow {
    background-color: rgba(0, 0, 0, 0.678);
    cursor: pointer;
}

.square-arrow:hover {
    background-color: rgba(0, 0, 0, 0.473);
}

.NavP {
    position: relative;
    left: 200px;
}

.top-logo {
    position: relative;
    top: -50px;
    left: -100px;
}

.demon-pri {
    position: relative;
    top: 200px;
    left: 300px;
}


.square {
    width: 70px;
    height: 70px;
    background-color: #fff;
    border-radius: 20%;

    margin-top: -50px;
}

.book-pub {
    position: absolute;
    bottom: 0px;
    right: -291px;
    height: 350px;
    width: 600px;
    background-color: #fff;
}

.bg-lightGreen {
    background-color: #00ff0009 !important;
}

.bg-lightGreen:hover {
    background-color: #ffffff !important;
}
</style>