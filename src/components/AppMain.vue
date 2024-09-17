<script>
import AppMainBanner from './AppMain/AppMainBanner.vue';
import AppMainListCards from './AppMain/AppMainListCards.vue';

export default {
  data(){
    return{

    }
  },
  components: {
    AppMainBanner,
    AppMainListCards,
  },
  methods: {

  },
}
</script>

<template>
  <main>
    <section>
      <div class="container"> 
          <AppMainListCards />
      </div>
    </section>
    <section class="bg-AppMainBanner">
      <div class="container">
        <AppMainBanner />
      </div>
    </section>
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