<template>
    <div class="our-help">
        <h1>{{pageName}}</h1>
        <p>{{pageDescription}}</p>
    </div>
</template>
<script>
export default {
    data:function () {
   return{
     pageName:"Blog",
     pageDescription:"This is  an blog page"
   };
 },
  name:"Help"
}
</script>