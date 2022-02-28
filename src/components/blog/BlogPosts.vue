<template>
    <div class="post-box">
        <span class="post-views">10</span>
        <h3 class="post-tital">Blog Post Tital</h3>
        <span class="post-date">2022-2-28</span>
        <p class="post-content">Ullamco minim aute reprehenderit nostrud qui consectetur sit quis laborum amet est ea. Commodo laboris elit cillum ea pariatur magna ex dolor excepteur cillum. Sunt consequat irure sunt nisi laboris irure est.
            qui qui laborum cupidatat ut nisi laborum magna dolore.
        </p>
        <div class="row">
            <div class="col-sm-6">
                <span class="post-auther">Post auther</span>
            </div>
            <div class="col-sm-6 text-right">
                <span class="post-category">Category Name</span>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name:"sidebar"
}
</script>
<style lang="scss" scoped>
.text-right{
    text-align: right !important;
}
.post-box{
    padding:15px;
    background-color: #FFF;
    box-shadow: 0 0 10px #DDD;
    position: relative;
    text-align: left;
    .post-views{
        position:absolute;
        right: 5px;
        top: 5px;
        background-color:rgb(4, 155, 84);
        border-radius: 4px;
        padding: 1px 5px;
        color:#fff;
        text-align: center;
        font-weight:bold ;
    }
    .post-date{
        display: block;
        font-size: 15px;
        color: #4a4646e8;
        padding: 0 0 5px;
    }
    .post-content{
        line-height: 1.8;
        color: rgba(0, 0, 0, 0.746)(0, 0, 0, 0.746);
    }
    .post-auther{
        background-color: #0a99b5;
        color: #fff;
        padding: 6px 10px;
        border-radius: 4px;
    }
    .post-category{
        background-color: #da0c27;
        color: #fff;
        padding: 6px 10px;
        border-radius: 4px;
    }
   
}

</style>