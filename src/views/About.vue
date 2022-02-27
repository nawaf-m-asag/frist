<template>
  <div class="about">
    <h1>{{pageName}}</h1>
    <p>{{pageDescription}}</p>
  </div>
</template>

<script>
//@ => src  

export default {
 data:function () {
   return{
     pageName:"About us",
     pageDescription:"This is  an about page"
  
   };
 },
  name:"about"
}
</script>
