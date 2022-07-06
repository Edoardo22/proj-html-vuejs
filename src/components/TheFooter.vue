<template lang="">
    
    <div class="jumbo-bg-footer container-fluid text-white">
         
        <div class="d-flex pt-5 ps-5">
            <div class="col-3 ps-5 pt-5">
         <img src="img/author-logo-round-200x205.png" alt="logo">
         </div>
         <div class="row w-100 pt-5 pb-5">
            <div class="col-3">
                <div class="fs-2 pb-5">ABOUT ME</div>
                <div class="text-off">Lorem ipsum dolor sit amet consectetur adipisicing elit. At ducimus, dolor non distinctio nobis cumque laudantium quam ex quas optio vero reprehenderit deserunt, illo nam, voluptas tenetur nihil provident expedita.</div>
            </div>
            <div class="col-3">
                <div class="fs-2 pb-4">ABOUT ME</div>
                <ul class="list-unstyled">
                <li v-for="(item,i) in linkList"  :key="i" class="py-1"><strong class="pe-4">></strong><a :href="item.url" class="text-decoration-none text-white">{{item.Testo}}</a></li>
                </ul>
            </div>
            <div class="col-3">
                <div class="fs-2 pb-4">ABOUT ME</div>
                <div>
                    <ul class="list-unstyled ">
                        <li v-for="(item,i) in infolist"  :key="i" class="py-1 text-off">{{item.Testo}}</li>
                    </ul>
                </div>
                <div>
                    <div v-for="(item,i) in socialList"  :key="i" :class="item.url" class="px-2 fs-5 icons"></div>
                </div>
            </div>
        </div>
        </div>
    <div class="text-center pt-5 pb-5 text-off">@ Copyright 2012 - 2020 | Avada Theme by <span class="text-white">ThemeFusion</span> | All Rights Reserved | Powered by <span class="text-white">Boolean</span> </div>
        </div>
 
   
     
       
    
</template>
<script>
export default {
    data() {
        return {
            linkList: [
                {
                    Testo: 'Lastest Books',
                    url: '/'
                },
                {
                    Testo: 'Upcoming Events',
                    url: '/'
                },
                {
                    Testo: 'Recent Articles',
                    url: '/'
                },
                {
                    Testo: 'Business Enquiries',
                    url: '/'
                },
                {
                    Testo: 'Visit My Foundation',
                    url: '/'
                }
            ],
            infolist: [
                {
                    Testo: '63 E. Studebaker  Street Bolingbrook, IL 60440'
                },
                {
                    Testo: 'Phone: (847)754-8989'
                },
                {
                    Testo: 'mobile: (847)376-4234'
                },
                {
                    Testo: 'Email:info@your-company.com'
                }
            ],
            socialList: [
                {

                    url: 'fa-brands fa-facebook-f'
                },
                {

                    url: 'fa-brands fa-twitter'
                },
                {

                    url: 'fa-brands fa-instagram'
                },
                {

                    url: 'fa-brands fa-linkedin-in'
                },
                {

                    url: 'fa-brands fa-youtube'
                }
            ]
        }
    }
}
</script>


<style lang="scss">
.jumbo-bg-footer {
    background-image: url("../../public/img/hero-07-2x.jpg");
    background-size: cover;
    background-repeat: no-repeat;
}

.jumbo-bg-footer::before {
    filter: brightness(0.7);
}
</style>