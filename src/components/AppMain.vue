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
    <p>
      {{ message }}
    </p>
  </main>
</template>


<style lang="scss" scoped>

  main{
    background-color: #1C1C1C;

    p{
      color: white;
      padding: 30px 0;
    }
  }

</style>