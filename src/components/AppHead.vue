<script>
export default {
  data(){
    return{
        headerListNav : [
            {name: 'characters', status: false},
            {name: 'comics', status: false},
            {name: 'movies', status: false},
            {name: 'tv', status: false},
            {name: 'games', status: false},
            {name: 'collectibiles', status: false},
            {name: 'videos', status: false},
            {name: 'fans', status: false},
            {name: 'news', status: false},
            {name: 'shop', status: false},
        ]
    }
  },
  components: {

  },
  methods: {

  },
}
</script>

<template>
    <header>
        <!-- logo -->
        <a href="#"><img src="../assets/img/dc-logo.png" alt="dc-logo"></a>
        
        <!-- list links -->
        <nav>
            <ul id="list-links">
                <li v-for="link in headerListNav">
                    <a href="#"><span>{{ link.name }}</span></a>
                </li>
            </ul>
        </nav>
    </header>
</template>


<style lang="scss" scoped>


</style>