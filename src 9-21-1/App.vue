<template>
  <div id="app">
    <!-- <router-link to='/home' tag="button" replace active-class="active">首页</router-link>
     <router-link to='/about' tag="button" replace active-class="active">关于</router-link> -->

      <router-link to='/home' tag="button" replace >首页</router-link>
     <router-link to='/about' tag="button" replace >关于</router-link>
       <router-link :to="'/user/'+userid" tag="button" replace >用户</router-link>
     <router-view></router-view>
     
  </div>
</template>

<script>
export default{
   name:'App',

  data(){
    return{
      userid:"111"
    }
  }
}

</script>

<style>
.active{
  color:purple;
}

</style>
