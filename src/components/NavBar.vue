<template lang="">
    <div class="">
        <ul v-for="(item,i) in NavList"  :key="i">
            <li>
                <a :href="item.url">{{item.name}}</a>
            </li>
          
        </ul>
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
                    name: 'Publications',
                    url: '/publications'
                },
                {
                    name: 'Reviews',
                    url: '/reviews'
                },
                {
                    name: 'Events',
                    url: '/events'
                },
                {
                    name: 'News',
                    url: '/news'
                },
                {
                    name: 'About',
                    url: '/about'
                },
                {
                    name: 'Articles',
                    url: '/articles'
                }
            ]
        }
    }
}
</script>


<style lang="scss">
</style>