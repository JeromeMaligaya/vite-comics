<script>
export default {
  data(){
    return{
        iconList: [
            {image:'footer-facebook.png'},
            {image:'footer-periscospe.png'},
            {image:'footer-pinterest.png'},
            {image:'footer-twitter.png'},
            {image:'footer-youtube.png'},
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
    <div id="footer-bottom">
        <div class="container">
            <a href="#">SIGN-UP NOW!</a>
            <div class="social">
                <p>FOLLOW US</p>
                <ul>
                    <li v-for="icon in iconList">
                        <a href="#"><img :src="`../../assets/img/${icon.image}`" :alt="`${icon.image}`"></a>
                    </li>
                </ul>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
#footer-bottom{
    background-color: black;

    img{
        color: red;
    }
}

</style>