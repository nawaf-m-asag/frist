<template>
  <div class="home">
    <form action="">
        <input :type="inputType">
        <button @click.prevent="switchPassWord">SHOW</button>
    </form>
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: "Home",
  data:function () {
   return{
    inputType:"password"
      };
  },

  methods: {
    switchPassWord(){
      this.inputType=this.inputType=="password"?"text":"password";
    }
  },
};
</script>

<style lang="scss" scoped>
form{
  margin-top: 200px;
  input,button{
    height: 40px;
  }
}

</style>