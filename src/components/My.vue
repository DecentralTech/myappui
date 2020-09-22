<template>
  <section>
    <div class="wrapper">
      <div class="title">
        <div class="cross"></div>
        <div class="hot">我的书籍</div>
        <div class="total">共上传5本书籍</div>
      </div>
      <div class="content">
        <div class="item">
          <div class="img-wrapper">
            <img src="../../static/bookCover2.png" />
          </div>
          <div class="item-name">庆余年</div>
          <span class="introduce">烧烤炸鸡啤酒</span>
        </div>
        <div class="item">
          <div class="img-wrapper">
            <img src="../../static/bookCover1.png" />
          </div>
          <div class="item-name">庆余年</div>
          <span class="introduce">烧烤炸鸡啤酒</span>
        </div>
        <div class="item">
          <div class="img-wrapper">
            <img src="../../static/bookCover3.png" />
          </div>
          <div class="item-name">庆余年</div>
          <span class="introduce">烧烤炸鸡啤酒</span>
        </div>
        <div class="item">
          <div class="img-wrapper">
            <img src="../../static/bookCover2.png" />
          </div>
          <div class="item-name">庆余年</div>
          <span class="introduce">烧烤炸鸡啤酒</span>
        </div>
        <div class="item">
          <div class="img-wrapper">
            <img src="../../static/bookCover1.png" />
          </div>
          <div class="item-name">庆余年</div>
          <span class="introduce">烧烤炸鸡啤酒</span>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style scoped>
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
  background-image: linear-gradient(to bottom, #fb5530, #fff);
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
  width: 33.3%;
  padding-bottom: 6px;
}
.item:nth-child(3n + 1) {
  padding-right: 4px;
}
.item:nth-child(3n-1) {
  padding-left: 4px;
  padding-right: 4px;
}
.item:nth-child(3n) {
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

</style>