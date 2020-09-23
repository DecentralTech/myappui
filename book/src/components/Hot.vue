<template>
  <section>
    <div class="wrapper">
      <div class="title">
        <div class="cross"></div>
        <div class="hot">Popular Books</div>
      </div>
      <div class="content">
        <div class="item">
          <div class="img-wrapper">
            <img src="../../static/bookCover1.png" />
          </div>
          <div class="item-name">The Second Coming of Christ</div>
          <span class="introduce">by Robert E. Speer</span>
        </div>
        <div class="item">
          <div class="img-wrapper">
            <img src="../../static/bookCover2.png" />
          </div>
          <div class="item-name">The Political History of the Devil</div>
          <span class="introduce">by Daniel Defoe</span>
        </div>
        <div class="item">
          <div class="img-wrapper">
            <img src="../../static/bookCover3.png" />
          </div>
          <div class="item-name">Secrets of Mental Supremacy</div>
          <span class="introduce">by William Richard Cunningham Latson</span>
        </div>
        <div class="item">
          <div class="img-wrapper">
            <img src="../../static/bookCover4.png" />
          </div>
          <div class="item-name">Thought Power</div>
          <span class="introduce">by Annie Wood Besant</span>
        </div>
        <div class="item">
          <div class="img-wrapper">
            <img src="../../static/bookCover5.png" />
          </div>
          <div class="item-name">Aryan Sun-Myths</div>
          <span class="introduce">by Sarah Elizabeth Titcomb</span>
        </div>
        <div class="item">
          <div class="img-wrapper">
            <img src="../../static/bookCover6.png" />
          </div>
          <div class="item-name">Logic, in Three Books</div>
          <span class="introduce">by Hermann Lotze</span>
        </div>
      </div>
      <!-- <div class="no-content">
          <div class="no-img">
              <img src="../../static/noBook.png" alt="">
          </div>
          <div class="no-tip">No Books</div>
      </div>-->
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
.content {
  width: 100%;
  display: flex;
  flex-wrap: wrap;
}
.item {
  width: 33.3%;
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
  height: 128px;
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
  display: inline-block;
  width: 100%;
  font-size: 12px;
  color: rgba(129, 129, 129, 0.7);
  overflow: hidden;
  text-overflow: ellipsis;
  white-space: nowrap;
}
.no-content {
  width: 100%;
}
.no-img {
  width: 40%;
  margin: auto;
  height: 160px;
  display: flex;
  justify-content: center;
  align-items: center;
}
.no-img > img {
  display: block;
  width: 100%;
}
.no-tip {
  text-align: center;
  color: #222222;
}
</style>