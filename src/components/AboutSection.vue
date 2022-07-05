<template lang="">
    <div class="fluid-container py-5">
        <div class="text-center">
         <div class="fs-2 pb-3">Dig a Little Deeper  Into Damon Vaughn</div>
          <div class="text-success pb-5">FIND OUT MORE ABOUT THE AUTHOR HIMSELF</div>
        </div>
   <div class="container d-flex">
    
    <div v-for="(item,i) in AboutList" class="about-img flex-grow-1 mx-4" :key="i" v-bind:style="{ backgroundImage: 'url(' + item.url + ')' }">
    <div class="text-center d-flex flex-column justify-content-end h-100 card-about">
    <div class="text-white pb-2 fs-3 ">{{item.titolo}}</div>
    <div class="w-25 border-bottom align-self-center"></div>
    <div class="text-warning pb-4 pt-3">{{item.testo}}</div>
    </div>
    </div>`
   </div>

     </div>
</template>
<script>
export default {
    data() {
        return {
            AboutList: [
                {
                    url: 'img/box-1.jpg',
                    titolo: 'About  Me',
                    testo: "Vestibulum ante ipsum primis"

                },
                {
                    url: 'img/box-3.jpg',
                    titolo: 'My Lastes Book',
                    testo: "Vestibulum ante ipsum primis"
                },
                {
                    url: 'img/box-4.jpg',
                    titolo: 'Book singing',
                    testo: "Vestibulum ante ipsum primis"
                },

            ]
        }
    }
}
</script>


<style lang="scss">
.about-img {
    border-bottom-right-radius: 16%;
    background-repeat: no-repeat;
    background-size: cover;
    background-position: center;
    height: 500px;
    filter: drop-shadow(2px 2px 2.5px black);
}

.card-about:hover {
    cursor: pointer;
    background: linear-gradient(to left, rgba(238, 238, 238, 0) 25%, rgba(0, 0, 0, 0.178) 50%, rgba(0, 0, 0, 0.233)) 75%, ;
}
</style>