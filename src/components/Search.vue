<template>
  <section>
    <div class="search">
      <input type="search" name="" class="sear">
      <img src="../static/search.png" alt="">
    </div>
  </section>
</template>

<script>
export default {
 methods:{
  //  search(){
  //    alert('1')
  //  }
 }
}
</script>

<style scoped>
 .search {
   /* width: 82px;
   height: 8px; */
   position: relative;
   
 }
 .search img{
   width: 16px;
   height: 16px;
   position: absolute;
   left: 9px;
   top:8px
 }
 .sear {
   width: 162px;
   height: 32px;
   border-radius: 16px;
   border:none;
   outline: none;
   text-indent: 2em;
 }
</style>