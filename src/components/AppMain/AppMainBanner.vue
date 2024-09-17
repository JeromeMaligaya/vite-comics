<script>
export default {
  data(){
    return{
        iconBannerList: [
            {iconUrl: 'buy-comics-digital-comics.png', label: 'digital comics'},
            {iconUrl: 'buy-comics-merchandise.png', label: 'dc merchandise'},
            {iconUrl: 'buy-comics-subscriptions.png', label: 'subscription'},
            {iconUrl: 'buy-comics-shop-locator.png', label: 'comic shop locator'},
            {iconUrl: 'buy-dc-power-visa.svg', label: 'dc power visa'},
        ]
    }
  },
  components: {

  },
  methods: {
    getImagePath(img){
        return new URL(`../../assets/img/${img}`, import.meta.url).href
    }
  },
}
</script>

<template>
    <ul class="banner-list">
        <li v-for="(item, index) in iconBannerList" :key="index">
            <a href="#"><img :src="getImagePath(item.iconUrl)" alt="`${item.iconUrl}`"></a>
            <span>{{ item.label.toUpperCase() }}</span>
        </li>
    </ul>

</template>

<style lang="scss" scoped>

</style>