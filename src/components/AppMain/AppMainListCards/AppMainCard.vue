<script>
export default {
  data(){
    return{

    }
  },
  props: {
    thumbUrl : {
        type: String,
        required: true,
    },
    price : {
        type: String,
        required: true,
    },
    series : {
        type: String,
        required: true,
    },
    type : {
        type: String,
        required: true,
    }

  },
  components: {

  },
  methods: {

  },
}
</script>

<template>
    <li class="card">
        <a href="#">
            <div class="img-box">
                <img :src="thumbUrl" :alt="thumbUrl" />
            </div>
        </a>
        <a href="#"><h3>{{ series }}</h3></a>
    </li>
</template>

<style lang="scss" scoped>
    @use "../../../style/general.scss" as *;
    
    .card {
        flex-basis: calc(100% / 6 - 90px / 6);

        .img-box{
            height: 150px;
            overflow: hidden;
        }
        h3{
            color: white;
            font-size: 10px;
            margin-top: 15px;
        }
    }

</style>
