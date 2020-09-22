<template>
  <div id="q-app">
    <p v-for='(item, index) of Object.keys(stuff)' :key="index">
      <span>{{ item }}</span>
      <span> -> -> -> </span>
      <span>{{ stuff[item] }}</span>
    </p>
  </div>
</template>
<script>
import { createPow } from '@textile/powergate-client'

export default {
  name: 'App',
  data() {
    return {
      stuff: {
        host: null,
        pow: null,
        status: null,
        messagesList: null,
        peersList: null,
        token: null,
      }
    }
  },
  async created() {
    // 创建实例
    this.stuff.host = 'https://slate.textile.io'
    this.stuff.pow = createPow({ host: this.stuff.host })

    // 不用授权，即可使用api
    const { status, messagesList } = await this.stuff.pow.health.check()
    this.stuff.status = status
    this.stuff.messagesList = messagesList
    this.stuff.peersList = await pow.net.peers()

    // 其他API需要授权。 您将与之交互的主要API是Filecoin文件系统（FFS），
    // 并且需要授权。 首先，创建一个新的FFS实例。
    const { token } = await this.stuff.pow.ffs.create()
    this.stuff.token = token

    // 当前，返回的身份验证令牌是唯一使您可以在以后访问FFS实例的事物
    // 因此请确保安全地保存它。
    // 拥有身份验证令牌后
    // 可以通过创建新的FFS实例或读取以前保存的实例
    // 来设置您希望Powergate客户端使用的身份验证令牌。

  }
}
</script>
