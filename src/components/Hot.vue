<template>
  <section>
    <div class="wrapper">
      <div class="title">
        <div class="cross"></div>
        <div class="hot">Popular uploads</div>
      </div>
      <div class="content">
        <div class="item">
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
        </div>
        <div class="item">
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
        </div>
        <div class="item">
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
  /* height: 103px; */
  /* position: absolute; */

  /* display: flex;
  justify-content: space-between;
  align-items: center; */
}
.img-wrapper > img {
  /* display: block; */
  width: 100%;
  /* height: 100%; */

}
.content-wrapper{
  /* margin-left: -90px; */
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
</style>