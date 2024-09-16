<script>
import AppFooterTop from './AppFooter/AppFooterTop.vue';
import AppFooterBottom from './AppFooter/AppFooterBottom.vue';

export default {
  data(){
    return{

    }
  },
  components: {
    AppFooterTop,
    AppFooterBottom,
  },
  methods: {

  },
}
</script>

<template>
  <footer>
    <AppFooterTop />
    <AppFooterBottom />
  </footer>
</template>


<style lang="scss" scoped>
@use "../style/general.scss" as *

</style>