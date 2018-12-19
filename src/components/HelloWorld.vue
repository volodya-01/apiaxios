<template>
  <div class="hello">
<!--    <demo/> -->
  </div>
</template>

<script>
/* import demo from '@/components/demo' */
export default {
  name: 'HelloWorld',
  components:{
    /* demo */
  },
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  },
  mounted(){
    this.$api.upload()
.then(res => {
/*   let self=this */
console.log(res);

});
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
