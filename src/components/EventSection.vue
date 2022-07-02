<template lang="">
    <div class="fluid-container pt-5 pb-5 bg-sand">
      <div class="fs-2 text-center py-3"> <strong>Upcoming Events</strong></div>
      <div class="text-center text-warning pb-5">MEET THE AUTHOR IN PERSON</div>
      <div class="container">
        <div class="row justify-content-between d-flex">
            <div class="card col-3 text-center px-0 mx-5" v-for="(event,i) in EventList"  :key="i">
               <img :src="event.url" class="card-img-top" alt="...">
               <div class="card-body">
                 <h5 class="card-title border-bottom py-4">{{event.titolo}}</h5>
                 <p class="card-text py-4 pb-3">{{event.testo}}</p>
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
            EventList: [
                {
                    url: 'img/event-05.jpg',
                    titolo: 'Chicago Book Singning',
                    testo: "in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum."

                },
                {
                    url: 'img/event-04.jpg',
                    titolo: 'Meet & Greet With Amanda',
                    testo: "in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum."
                },
                {
                    url: 'img/event-07.jpg',
                    titolo: 'Open Book Dialogues',
                    testo: "in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum."
                },

            ]
        }
    }
}
</script>


<style lang="scss">
</style>