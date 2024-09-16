<script>
export default {
  data(){
    return{
        footerList:[
            {
                title: 'DC COMICS',
                items: [
                    {name:'Characters' , status: true},
                    {name:'Comics' , status: true},
                    {name:'Movies' , status: true},
                    {name:'TV' , status: true},
                    {name:'Games' , status: true},
                    {name:'Videos' , status: true},
                    {name:'Nwes' , status: true},
                ]
            },
            {
                title: 'SHOP',
                items: [
                    {name:'Shop DC' , status: true},
                    {name:'Shop DC Collectbles' , status: true},
                ]
            },
            {
                title: 'DC',
                items: [
                    {name:'Teams Of Use' , status: true},
                    {name:'Privacy policy(New)' , status: true},
                    {name:'Ad Choices' , status: true},
                    {name:'Advertising' , status: true},
                    {name:'Jobs' , status: true},
                    {name:'Subscriptions' , status: true},
                    {name:'Talent Workshop' , status: true},
                    {name:'CPSC Certificates' , status: true},
                    {name:'Ratings' , status: true},
                    {name:'Shop Help' , status: true},
                    {name:'Contact Us' , status: true},
                ]
            },
            {
                title: 'SITES',
                items: [
                    {name:'DC' , status: true},
                    {name:'MAD Magazine' , status: true},
                    {name:'DC Kids' , status: true},
                    {name:'DC Universe' , status: true},
                    {name:'DC Power Visa' , status: true},
                ]
            },
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
    <div class="container">
        <div id="footer-bottom" v-for="element in footerList">
            <div class="card-footer">
                <h3>{{ element.title }}</h3>
                <ul>
                    <li v-for="item in element.items">
                        <span>{{ item.name }}</span>
                    </li>
                </ul>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use "../../style/general.scss" as *;

</style>