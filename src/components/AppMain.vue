<script>
export default {
  data(){
    return{
      message: '--> Content goes here <--'
    }
  },
  components: {

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
  </main>
</template>


<style lang="scss" scoped>

  main{
    background-color: #1C1C1C;

    p{
      color: white;
      padding: 30px 0;
      font-size: 20px;
      font-weight: bold
    }
  }

</style>