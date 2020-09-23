<template>
    <section>
        <div class="wrapper">
            <div>Shared Books</div>
            <span>Share your favorite books</span>

            <div class="search-wrapper">
                <div class="icon-wrapper">
                    <img src="../../static/search.png" alt="">
                </div>
                <div class="input">
                    <input type="text" placeholder="please search">
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    
}
</script>

<style scoped>
.wrapper{
    padding-top: 50px;
    padding-left: 20px;
    position: relative;
}
.wrapper>div{
    font-size: 20px;
    color: #fff;
    font-weight: 500;
}
.wrapper>span{
    color: rgba(255, 255, 255,0.7);
}
.search-wrapper{
    width: 160px;
    height: 32px;
    position: absolute;
    right: 5vw;
    top:60px;
    background-color: #fff;
    display: flex;
    border-radius: 20px;
}
.icon-wrapper{
    width: 32px;
    display: flex;
    justify-content: center;
    align-items: center;
}
.icon-wrapper>img{
    display: block;
    width: 18px;
}
.input{
    flex: 1;
}
.input>input{
    font-size: 14px;
    width: 120px;
    outline: none;
    border-radius: 10px;
    border: none;
    color: #9297A2;
}
::-webkit-input-placeholder { /* WebKit browsers */
  color: #9297A2;
  font-weight: 400;
}

::-moz-placeholder { /* Mozilla Firefox 19+ */
  color: #9297A2;
  font-weight: 400;
}

:-ms-input-placeholder { /* Internet Explorer 10+ */
  color: #9297A2;
  font-weight: 400;
}  
</style>