<template>
  <section>
    <div class="wrapper">
      <div class="title">
        <div class="cross"></div>
        <div class="hot">My video</div>
        <div class="total">4 videos uploaded</div>
      </div>
      <!-- <div class="content">
        <div class="item">
          <div class="img-wrapper">
            <img src="../static/picture1.png" />
          </div>
          <div class="item-name">WWE第1246期</div>
          <span class="introduce">精彩回放</span>
        </div>
        <div class="item">
          <div class="img-wrapper">
            <img src="../static/picture3.png" />
          </div>
          <div class="item-name">全国21日新增6例确诊</div>
          <span class="introduce">境外输入</span>
        </div>
        <div class="item">
          <div class="img-wrapper">
            <img src="../static/picture2.png" />
          </div>
          <div class="item-name">极限挑战宝藏行</div>
          <span class="introduce">魏大勋刘宇宇抢人大战</span>
        </div>
         <div class="item">
          <div class="img-wrapper">
            <img src="../static/picture4.png" />
          </div>
          <div class="item-name">刘宇定最美逆行者</div>
          <span class="introduce">OST来袭：感谢所有逆行者</span>
        </div>
      </div> -->


      <ul class="content">
        <template v-if="0">
          <li class="item">
            <div class="img-wrapper">
              <img src="../static/picture1.png" />
            </div>
            <div class="item-name">WWE第1246期</div>
            <span class="introduce">精彩回放</span>
          </li>
          <li class="item">
            <div class="img-wrapper">
              <img src="../static/picture3.png" />
            </div>
            <div class="item-name">全国21日新增6例确诊</div>
            <span class="introduce">境外输入</span>
          </li>
          <li class="item">
            <div class="img-wrapper">
              <img src="../static/picture2.png" />
            </div>
            <div class="item-name">极限挑战宝藏行</div>
            <span class="introduce">魏大勋刘宇宇抢人大战</span>
          </li>
          <li class="item">
            <div class="img-wrapper">
              <img src="../static/picture4.png" />
            </div>
            <div class="item-name">刘宇定最美逆行者</div>
            <span class="introduce">OST来袭：感谢所有逆行者</span>
          </li>
        </template>
        <li v-else class="item1">
           <img src="../static/notFind.png" alt="" class="notlogo">
        </li>
      </ul>
    </div>
  </section>
</template>

<script>
export default {
  data: {
    list: [

    ]
  }

};
</script>

<style scoped>
*{ margin:0; padding:0; }
.wrapper {
  width: 90vw;
  margin: auto;
}
.title {
  height: 32px;
  line-height: 32px;
  display: flex;
  position: relative;
}
.cross {
  width: 5px;
  height: 16px;
  background-image: linear-gradient(to bottom, rgb(12, 119, 190), #fff);
  position: absolute;
  top: 8px;
  border-radius: 10px;
}
.hot {
  flex: 1;
  padding-left: 12px;
  font-weight: 600;
}
.total{
  font-size: 13px;
}
.content {
  width: 100%;
  display: flex;
  flex-wrap: wrap;
}
.item {
  width: 50%;
  padding-bottom: 6px;
}
.item:nth-child(2n-1) {
  padding-right: 4px;
}
.item:nth-child(2n) {
  padding-left: 4px;
}
.img-wrapper {
  height: 103px;
  display: flex;
  justify-content: center;
  align-items: center;
}
.img-wrapper > img {
  display: block;
  width: 100%;
  height: 100%;
}
.item-name {
  font-size: 14px;
  font-weight: 600;
  padding-top: 4px;
  overflow: hidden;
  text-overflow: ellipsis;
  white-space: nowrap;
}
.introduce {
  font-size: 12px;
  color: rgba(129, 129, 129, 0.7);
  overflow: hidden;
  text-overflow: ellipsis;
  white-space: nowrap;
}
ul{
  position: relative;
}
li{
  list-style: none;
}
.notlogo {
  width: 90px;
  height: 59px;
}
.item1{
 display: inline;
 margin:10px auto;
}
</style>