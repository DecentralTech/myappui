<template>
    <section class="container">
        <div class="wrapper">
            <div>Share Linux image</div>
            <span>Share your favorite Linux image</span>
        </div>
        <div class="search">
           <input type="search" name="" class="sear" placeholder=" search">
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
}
.wrapper>div{
    font-size: 20px;
    color: #fff;
    font-weight: 500;
}
.wrapper>span{
    color: rgba(255, 255, 255,0.7);
    font-size: 12px;
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
   /* width: 162px; */
   width: 113px;
   height: 32px;
   border-radius: 16px;
   border:none;
   outline: none;
   text-indent: 2em;
 }
</style>