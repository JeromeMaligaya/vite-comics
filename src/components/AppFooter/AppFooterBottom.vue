<script>
export default {
  data(){
    return{
        iconList: [
            {image:'footer-facebook.png'},
            {image:'footer-periscope.png'},
            {image:'footer-pinterest.png'},
            {image:'footer-twitter.png'},
            {image:'footer-youtube.png'},
        ]
    }
  },
  components: {

  },
  methods:{
    getImagePath(img){
        return new URL(`../../assets/img/${img}`, import.meta.url).href
    }

  },
}
</script>

<template>
    <div id="footer-bottom">
        <div class="container">
            <a class="btn" href="#">SIGN-UP NOW!</a>
            <div class="social">
                <p>FOLLOW US</p>
                <ul>
                    <li v-for="icon in iconList">
                        <a href="#"><img :src="getImagePath(icon.image)" :alt="`${icon.image}`"></a>
                    </li>
                </ul>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
#footer-bottom{
    background-color: #303030;

    .container{
        display: flex;
        align-items: center;
        justify-content: space-between;
        padding: 20px 0;

        a.btn{
            color: white;
            border: 2px solid #0282F9;
            padding: 5px;
        }

        .social{
        display: flex;
        align-items: center;

        p{
          color:#0282F9;
          margin-right: 10px;  
        }

        ul{
            display: flex;
            gap: 10px;
        }
    }
    }
}

</style>