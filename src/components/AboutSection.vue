<template lang="">
    <div class="fluid-container py-5">
        <div class="text-center">
         <div class="fs-2 pb-3">Dig a Little Deeper  Into Damon Vaughn</div>
          <div class="text-success pb-5">FIND OUT MORE ABOUT THE AUTHOR HIMSELF</div>
        </div>
   <div class="container d-flex">
    <div v-for="(item,i) in AboutList"  :key="i" class="position-relative">
   
    <img :src="item.url" alt="" class="about-img w-75 h-100">
    <div class="text-light pb-2 ">About Me</div>
    
    </div>
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
    position: relative;
}
</style>