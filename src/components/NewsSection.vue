<template lang="">
    <div class="fluid-container pt-5 pb-5 bg-newsletter text-center d-flex justify-content-center">
        <div class="row d-flex justify-content-center">
            <div class="col-8 ">
     <div class="text-light fs-2 py-3 pt-5">Subscribe To My Newsletter</div>
     <div class="text-warning pb-4">BE NOTIFIED ABOUT BOOK SINGING TOUR DATES</div>
     <div class="d-flex justify-content-center">
     <input type="email" class="rounded border-0 me-3 px-2" placeholder="insert your email ..*">
     <button class="btn btn-success px-3 py-1 flex-grow-1" @click="subText">Subscribe</button>
     </div>
     <div class="text-light py-5" v-if="!subscribe">Donec fringilla nunc eu turpis dignissim, at euismod sapien tincidunt.</div>
     <div class="text-light py-5" v-else>Grazie di esserti iscritto alla nostra News Letter! Riceverai solo le mail importanti, <br> niente spam.</div>
  </div>
  </div>
   </div>
    
</template>
<script>
export default {
    data() {
        return {
            subscribe: false,
        }
    },
    methods: {
        subText() {
            this.subscribe = true;
        }
    }
}
</script>


<style lang="scss">
.bg-newsletter {
    background-image: url('../../public/img/banner-2.jpg');
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;

}
</style>