<script>
import AppHeader from './components/AppHead.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';

export default {
  data(){
    return{

    }
  },
  components: {
    AppHeader,
    AppMain,
    AppFooter,
  },
  methods: {

  },
}
</script>

<template>
  <AppHeader />
  <AppMain />
  <AppFooter />
</template>

<style lang="scss">
@use "./style/general.scss" as *;

</style>
