<template>
    <div class="header">
        <div class="container">
            <div class="logo">App Logo</div>
            <ul>
                <router-link to="/" tag="li" exact>
                    <li><a>Home</a></li>
                </router-link>
                <router-link to="/blog" tag="li" exact>
                    <li><a>Blog</a></li>
                </router-link>  
                <router-link to="/about" tag="li">
                <li><a>About</a></li>
                </router-link> 
                <router-link to="/help"  tag="li" replace>
                    <li><a>Help</a></li>
                </router-link>
            </ul>
        </div>
    </div>
</template>
<script>
export default {
    name:"AppHeader"
}
</script>
<style lang="scss" scoped>
    .header{
        background: #333;
        color:#fff;
        overflow: hidden;
        height: 60px;
        position: fixed;
        top: 0;
        right: 0;
        width: 100%;
        z-index: 1000;
        .logo{
            font-size: 24px;
            padding: 20px;
            float: left;
            width: 200px;
            }
        ul {
        margin-top: 10px;    
        float: left;
        width: calc(100% - 200px);
        height: 40;
        li {
            padding: 10px;
            display: inline-block;
            font-size: 18px;

               a {
                    color: #fff;
                    text-decoration: none;
                 }
               
            }
        }
        .router-link-exact-active li{
            background:rgb(226, 5, 5) !important;
            border-radius: 5px;
        } 
    }
   
    
    
 
</style>