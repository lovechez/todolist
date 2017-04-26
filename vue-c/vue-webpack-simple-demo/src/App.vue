<template>
  <div id="app">
    <h1>{{ msg }}</h1>
    <input type="button" value="change" @click="change">
  </div>
</template>

<script>
export default {
  data () {
    return {
      msg: 'Hello Vue1!'
    }
  },
  methods:{
    change(){
      this.msg= this.msg.split('').reverse().join('');;
    }
  }

}
</script>

<style>
body {
  font-family: Helvetica, sans-serif;
}
</style>
