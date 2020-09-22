<template>
  <section>
    <div class="upload">
      <label>upload</label>
      <input type="file" class="file" />
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style scoped>
.upload {
  width: 50vw;
  height: 36px;
  line-height: 36px;
  background-image: linear-gradient(to right, #436fc2, rgb(12, 119, 190));
  margin: 20px auto;
  border-radius: 20px;
  position: relative;
  text-align: center;
  color: #fff;
}
.file {
  width: 100%;
  height: 100%;
  position: absolute;
  left: 0;
  right: 0;
  opacity: 0;
}
</style>