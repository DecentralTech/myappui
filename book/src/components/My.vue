<template>
  <section>
    <div class="wrapper">
      <div class="title">
        <div class="cross"></div>
        <div class="hot">Sharing Books</div>
        <div class="total">A total of 5 books</div>
      </div>
      <!-- <div class="content">
        <div class="item">
          <div class="img-wrapper">
            <img src="../../static/bookCover7.png" />
          </div>
          <div class="item-name">The Lost Lemuria</div>
          <span class="introduce">by W. Scott-Elliot</span>
        </div>
        <div class="item">
          <div class="img-wrapper">
            <img src="../../static/bookCover8.png" />
          </div>
          <div class="item-name">Atlantis</div>
          <span class="introduce">by Ignatius Donnelly</span>
        </div>
        <div class="item">
          <div class="img-wrapper">
            <img src="../../static/bookCover9.png" />
          </div>
          <div class="item-name">A Guide to Mythology</div>
          <span class="introduce">by Helen Archibald Clarke</span>
        </div>
        <div class="item">
          <div class="img-wrapper">
            <img src="../../static/bookCover12.png" />
          </div>
          <div class="item-name">Moon Lore</div>
          <span class="introduce">by Timothy Harley</span>
        </div>
        <div class="item">
          <div class="img-wrapper">
            <img src="../../static/bookCover11.png" />
          </div>
          <div class="item-name">Why the Mind Has a Body</div>
          <span class="introduce">by Charles Augustus Strong</span>
        </div>
        <div class="item">
          <div class="img-wrapper">
            <img src="../../static/bookCover10.png" />
          </div>
          <div class="item-name">Our Story of Atlantis</div>
          <span class="introduce">by William P. Phelon</span>
        </div>
      </div> -->
      <div class="no-content">
          <div class="no-img">
              <img src="../../static/noBook.png" alt="">
          </div>
          <div class="no-tip">No Books</div>
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
.no-content{
    width: 100%;
}
.no-img{
    width: 40%;
    margin: auto;
    height: 160px;
    display: flex;
    justify-content: center;
    align-items: center;
}
.no-img>img{
    display: block;
    width:100%;
}
.no-tip{
    text-align: center;
    color: #222222;
}
</style>