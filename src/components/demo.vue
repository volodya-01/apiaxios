<template>
    <div>{{msg}}</div>
</template>
<script>
export default {
    name:"demo",
      data(){
            return{
              msg:[]
            }
        },
        created(){
             let self = this;
      self.$axios
        .post("https://112.64.170.158:8187/Service1.svc/CJConditionSetting")
        .then(function(res) {
          console.log(res);
          self.msg=res
        })
        .catch(function(err) {
          console.log(err);
        })
        }
}
</script>

