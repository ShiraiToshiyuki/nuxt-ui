<template>
<div>
  <v-badge>{{$store.state.counter}}</v-badge>
  <v-btn color="primary" @click="this.countUp">ボタン</v-btn>
</div>
</template>

<script>
export default {
  name: "test",
  methods:{
    countUp(){
      this.$store.commit('increment')
    }
  }
}


</script>

<style scoped>

</style>
