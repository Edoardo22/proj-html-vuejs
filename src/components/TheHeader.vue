<template lang="">
    <div class="jumbo-bg container-fluid d-flex justify-content-center">
        <div class="row container pt-5  position-relative">
            <div class="col-6">
                <div>
                    <img src="img/author-logo-round-200x205.png" alt="logo" class="img-fluid top-logo">
                </div>
                <div class="text-warning pb-4 allura">Damon Vaugh</div>
              <div class="text-white fs-1 pb-4">Best-selling author and the most influential public intellectual in the western world right now.</div>  
              <div class="text-light fs-4">- The New York Times</div>
                </div>
             <div class="col-6 d-flex">
                <ul class="navbar-nav me-auto mb-2 mb-lg-0 NavP" v-for="(item,i) in NavList"  :key="i">
            <li>
                <a class="nav-item text-decoration-none text-white px-2" :href="item.url">{{item.name}}</a>
            </li>
            </ul>
             <div class="demon-pri">
                 <div class="square mb-4 text-center">Demos</div>
                  <div class="square mt-4 text-center">
                    <span class="align-top">$</span>
                    <span class="fs-2">39</span>
                    <div class="">On Sale</div>
                  </div>
            </div>
            <div class="book-pub">
                <div class="row">
                    <div class="col-6 d-flex justify-content-center pt-5 ps-5">
                        <img src="img/book-widget.png">
                    </div>
                    <div class="col-6 pt-5 pe-0">
                        <div class=" fs-4 pb-3">LASTEST BOOK RELEASE</div>
                        <div class="text-warning pb-3">D. VAUGHN AUTOBIOGRAPHY</div>
                          <div class="">Best-selling author and the most influential public intellectual in the western world right now.</div>
                    </div>
                </div>
                <div class="d-flex text-center justify-content-center">
                    <button type="button" class="btn btn-success px-5 py-2">Buy on Amazon</button>
                    <button type="button" class="btn btn-success px-5 py-2">Buy on App Store</button>
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
                    url: '/'
                },
                {
                    name: 'About Me',
                    url: '/About'
                },
                {
                    name: 'Testimonials',
                    url: '/Testimonials'
                },
                {
                    name: 'My Blog',
                    url: '/Blog'
                },
                {
                    name: 'Meetups',
                    url: '/Meetups'
                },
                {
                    name: 'Shop',
                    url: '/Shop'
                },
                {
                    name: 'Contact Me',
                    url: '/Contact'
                }
            ]
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
</style>