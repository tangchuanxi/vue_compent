<template>
  <div class="hello">
    <button @click="showToast">按钮</button> 
    <button @click="turnToTest">跳转</button> 
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  },
  methods: {
    showToast: function(){
      this.$toast("新内容", 1500);
    },
    turnToTest:()=>{
      this.$router.push("/test")
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
