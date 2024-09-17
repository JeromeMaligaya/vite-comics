<script>
import AppMainBanner from './AppMain/AppMainBanner.vue';
import AppMainCard from './AppMain/AppMainCard.vue';

export default {
  data(){
    return{
      message: '--> Content goes here <--'
    }
  },
  components: {
    AppMainBanner,
    AppMainCard,
  },
  methods: {

  },
}
</script>

<template>
  <main>
    <div class="container">
      <p>
        {{ message }}
      </p>
    </div>
    <div class="bg-AppMainBanner">
      <div class="container">
        <AppMainBanner />
      </div>
   </div>
  </main>
</template>


<style lang="scss">

  main{
    background-color: #1C1C1C;

    p{
      color: white;
      padding: 30px 0;
      font-size: 20px;
      font-weight: bold
    }

    .bg-AppMainBanner{
      background-color: rgb(2, 130, 249);
    }
  }

</style>