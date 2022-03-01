<template>
    <div class="our-help">
        <h1>{{pageName}}</h1>
        <p>{{pageDescription}}</p>
        <div class="container">
          <div class="row">
            <div class="col-md-8">
              <div class="post-area">
                <BlogPosts v-for="post in posts" v-bind:key="post.id" 
                :views="post.views"  
                :title="post.title"  
                :content="post.content"  
                :date="post.date"  
                :auther="post.auther"  
                :category="post.category"/>
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
import PostJson from '../json/BlogData.json';
export default {
  
    data:function () {
   return{
     pageName:"Blog",
     pageDescription:"This is  an blog page",
     posts:PostJson
   };
 },
  name:"Help",
  components:{
    BlogPosts,
    BlogSidebar,
    
  }
}
</script>