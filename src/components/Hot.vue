<template>
  <section>
    <div class="wrapper">
      <div class="title">
        <div class="cross"></div>
        <div class="hot">Hot Videos</div>
      </div>
      <div class="content">
        <div class="item">
          <div class="img-wrapper">
            <img src="../static/picture1.png" />
          </div>
          <div class="item-name">WWE 1246</div>
          <div class="introduce">Wonderful playback</div>
        </div>
        <div class="item">
          <div class="img-wrapper">
            <img src="../static/picture3.png" />
          </div>
          <div class="item-name">Six new cases were confirmed nationwide on the 21st</div>
          <div class="introduce">Overseas import</div>
        </div>
        <div class="item">
          <div class="img-wrapper">
            <img src="../static/picture2.png" />
          </div>
          <div class="item-name">Ultimate challenge treasure line</div>
          <div class="introduce">Wei daxun and Liu yuyu </div>
        </div>
         <div class="item">
          <div class="img-wrapper">
            <img src="../static/picture4.png" />
          </div>
          <div class="item-name">Liu Yuding is the most beautiful rebel</div>
          <div class="introduce">OST coming: Thank you to all those who are against it </div>
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
  /* width: 50%; */
  font-size: 14px;
  font-weight: 600;
  padding-top: 4px;
  overflow: hidden;
  text-overflow: ellipsis;
  white-space: nowrap;
}
.introduce {
  font-size: 12px;
  color: rgba(129, 129, 129,0.7);
  overflow: hidden;
  text-overflow: ellipsis;
  white-space: nowrap;
}
</style>