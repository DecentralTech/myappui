<template>
  <section>
    <div class="wrapper">
      <div class="title">
        <div class="cross"></div>
        <div class="hot">My upload</div>
        <div class="total">Upload 4 files</div>
      </div>
      <!-- <div class="content">
        <div class="item">
          <div class="img-wrapper">
            <img src="../static/flieLogo.png" />
          </div>
          <div class="content-wrapper">
            <div class="item-name">阿里云镜像资源站</div>
            <span class="introduce">5G</span>
          </div>
           <div class="date-wrapper">
            <div class="item-date">2020-05-26</div>
          </div>
        </div>
        <div class="item">
          <div class="img-wrapper">
            <img src="../static/flieLogo.png" />
          </div>
          <div class="content-wrapper">
            <div class="item-name">阿里云镜像资源站</div>
            <span class="introduce">5G</span>
          </div>
           <div class="date-wrapper">
            <div class="item-date">2020-05-26</div>
          </div>
        </div>
      </div> -->

      <ul class="content">
        <template v-if="0">
          <li class="item">
            <div class="img-wrapper">
              <img src="../static/flieLogo.png" />
            </div>
            <div class="content-wrapper">
              <div class="item-name">Alicloud image resource station</div>
              <span class="introduce">5G</span>
            </div>
            <div class="date-wrapper">
              <div class="item-date">2020-05-26</div>
            </div>
          </li>
          <li class="item">
            <div class="img-wrapper">
              <img src="../static/flieLogo.png" />
            </div>
            <div class="content-wrapper">
              <div class="item-name">Alicloud image resource station</div>
              <span class="introduce">5G</span>
            </div>
            <div class="date-wrapper">
              <div class="item-date">2020-05-26</div>
            </div>
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
export default {};
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
  margin-bottom: 8px;
}
.cross {
  width: 5px;
  height: 16px;
  background-image: linear-gradient(to bottom, rgb(12, 190, 51), #fff);
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
    width: 100%;
  /* padding-bottom: 6px; */
  /* position: relative; */
  margin-bottom: 12px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.img-wrapper {
  width: 55PX;
  height: 42px;
  /* height: 103px;
  display: flex;
  justify-content: center;
  align-items: center; */
}
.img-wrapper > img {
  /* display: block; */
  width: 100%;
  /* height: 100%; */
}
.content-wrapper{
  /* margin-left: -140px; */
  width: 50%;
  overflow: hidden;
  text-overflow: ellipsis;
  white-space: nowrap;
}
.content-wrapper .item-name {
  font-size: 14px;
  font-weight: 600;
  padding-top: 4px;
  overflow: hidden;
  text-overflow: ellipsis;
  white-space: nowrap;
}
.content-wrapper .introduce {
  font-size: 14px;
  color: #9297A2;
  overflow: hidden;
  text-overflow: ellipsis;
  white-space: nowrap;
}
.date-wrapper .item-date {
  font-size: 12px;
  color:#9297A2;
  margin-top:30px
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