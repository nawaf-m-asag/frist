<template>
    <div class="our-help">
        <h1>{{pageName}}</h1>
        <p>{{pageDescription}}</p>
        <div class="container">
          <div class="row">
            <div class="col-md-8">
              <div class="post-area">
                <BlogPosts />
              </div>
            </div>
            <div class="col-md-4">
              <div class="sidebar">
                  <BlogSidebar />
              </div>
            </div>
          </div>
        </div>
    </div>
</template>
<script>
import BlogPosts from '@/components/blog/BlogPosts';
import BlogSidebar from '@/components/blog/BlogSidebar';
export default {
  
    data:function () {
   return{
     pageName:"Blog",
     pageDescription:"This is  an blog page"
   };
 },
  name:"Help",
  components:{
    BlogPosts,
    BlogSidebar
  }
}
</script>