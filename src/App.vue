<template>
  <div id="q-app">
    <div class="top-container">
      <top-header></top-header>
      <banner class="banner"></banner>
    </div>
    <hot></hot>
    <my></my>
    <upload></upload>
  </div>
</template>
<script>
import { createPow } from "@textile/powergate-client";
import Banner from "./components/Banner";
import Hot from "./components/Hot";
import My from "./components/My";
import TopHeader from "./components/TopHeader";
import Upload from "./components/Upload";

export default {
  name: "App",
  components: {
    Banner,
    Hot,
    My,
    TopHeader,
    Upload,
  },
  data() {
    return {
      stuff: {
        host: null,
        pow: null,
        status: null,
        messagesList: null,
        peersList: null,
        token: null,
      },
    };
  },
  async created() {
    // 创建实例
    this.stuff.host = "https://slate.textile.io";
    this.stuff.pow = createPow({ host: this.stuff.host });

    // 不用授权，即可使用api
    const { status, messagesList } = await this.stuff.pow.health.check();
    this.stuff.status = status;
    this.stuff.messagesList = messagesList;
    this.stuff.peersList = await pow.net.peers();

    // 其他API需要授权。 您将与之交互的主要API是Filecoin文件系统（FFS），
    // 并且需要授权。 首先，创建一个新的FFS实例。
    const { token } = await this.stuff.pow.ffs.create();
    this.stuff.token = token;

    // 当前，返回的身份验证令牌是唯一使您可以在以后访问FFS实例的事物
    // 因此请确保安全地保存它。
    // 拥有身份验证令牌后
    // 可以通过创建新的FFS实例或读取以前保存的实例
    // 来设置您希望Powergate客户端使用的身份验证令牌。
  },
};
</script>

<style scoped>
.top-container{
  width: 100vw;
  background-image: url('../static/background.png');
  background-size: cover;
  /* border-bottom-left-radius: 10%;
   border-bottom-right-radius: 10%; */
}
.banner{
  padding-top: 20px;
}
</style>
