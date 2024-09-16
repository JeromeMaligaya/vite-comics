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
        ],
        currentIndex : null,
    }
  },
  components: {

  },
  methods: {
    selectLink(index){
        this.currentIndex = index;
    }
  },
}
</script>

<template>
    <header>
        <!-- logo -->
        <a href="#" class="img-box"><img src="../assets/img/dc-logo.png" alt="dc-logo"></a>
        
        <!-- list links -->
        <nav>
            <ul id="list-links">
                <li v-for="(link, index) in headerListNav" @click="selectLink(index)" :class="{ active : currentIndex === index}">
                    <a href="#"><span>{{ link.name.toUpperCase() }}</span></a>
                </li>
            </ul>
        </nav>
    </header>
</template>


<style lang="scss" scoped>

    header{
        display: flex;
        align-items: center;
        justify-content: space-between;

        .img-box{
            height: 75px;
            width: 75px;
        }

        nav, #list-links, #list-links li{
            height: 100%;
        }

        #list-links{
            display: flex;
        }

        #list-links li{
            padding: 15px;
        }

        li.active{
           
            border-bottom: solid 5px;
                border-color: blue;
            a span{
                color: blue;
                
            }
        }
    }

</style>