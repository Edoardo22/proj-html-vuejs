<template lang="">
    <div class="fluid-container  bg-sand d-flex justify-content-center py-5">
        <div v-for="(brand,i) in brandList"   :key="i" class="px-4"> <img :src="brand.url" :alt="brand.name">  </div>
       
        </div>
    
    
</template>
<script>
export default {
    data() {
        return {
            brandList: [
                {
                    name: 'ebay',
                    url: 'img/ebay-logotan-2x-200x66.png'
                },
                {
                    name: 'audible',
                    url: 'img/audible-logotan-2x-200x66.png'
                },
                {
                    name: 'barnesNoble',
                    url: 'img/bb-logotan-2x-200x66.png'
                },
                {
                    name: 'kindle',
                    url: 'img/kindlefire-logotan-2x-200x66.png'
                },

            ]

        }
    }
}
</script>


<style lang="scss">
.bg-sand {
    background-color: rgb(254, 247, 233);
}
</style>
