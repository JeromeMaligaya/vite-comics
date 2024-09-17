<script>
export default {
  data(){
    return{

    }
  },
  components: {

  },
  methods: {

  },
}
</script>

<template>
    <div class="jumbotron">
        <div class="container">
        <p class="current-series-badge">CURRENT SERIES</p>
    </div>
    </div>
</template>

<style lang="scss" scoped>

    .jumbotron{
        background-image: url(../../assets/img/jumbotron.jpg);
        background-position: top;
        background-size: cover;
        height: 300px;
        
        .current-series-badge{
            color: white;
            background-color: rgb(2, 130, 249);
            font-size: 15px;
            display: inline-block;
            padding: 5px 15px;
            position: relative;
            top:288px;
        }
    }

</style>
