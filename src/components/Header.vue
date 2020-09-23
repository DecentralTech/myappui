<template>
    <section class="container">
        <div class="wrapper">
            <div>Share video</div>
            <span>Share your favorite videos</span>
        </div>
        <div class="search">
           <input type="search" name="" class="sear" placeholder="Please search">
           <img src="../static/search.png" alt="">
        </div>
    </section>
</template>

<script>
export default {
    
}
</script>

<style scoped>
.container {
    display: flex;
    justify-content: space-around;
    align-items: flex-end;
}
.wrapper{
    padding-top: 50px;
    padding-left: 20px;
    flex-shrink: 1;
}
.wrapper>div{
    font-size: 20px;
    color: #fff;
    font-weight: 500;
}
.wrapper>span{
    color: rgba(255, 255, 255,0.7);
}
.search {
   /* width: 82px;
   height: 8px; */
   position: relative;
   /* flex-basis: auto; */
   flex-shrink: 1;
   padding-right: 20px;
 }
 .search img{
   width: 16px;
   height: 16px;
   position: absolute;
   left: 9px;
   top:8px
 }
 .sear {
   /* flex-shrink: 1; */
   width: 162px;
   height: 32px;
   border-radius: 16px;
   border:none;
   outline: none;
   text-indent: 2em;
 }
</style>