<template>
  <div class="contact-us">
    <div class="contact-us-title">代码与应用安全专家</div>
    <div class="contact-us-phone">联系我们</div>
  </div>
</template>

<script>
export default {
  components: {},
  props: {},
  data() {
    return {};
  },
  computed: {},
  watch: {},
  methods: {},
  created() {},
  mounted() {},
  beforeCreate() {}, // 生命周期 - 创建之前
  beforeMount() {}, // 生命周期 - 挂载之前
  beforeUpdate() {}, // 生命周期 - 更新之前
  updated() {}, // 生命周期 - 更新之后
  beforeDestroy() {}, // 生命周期 - 销毁之前
  destroyed() {}, // 生命周期 - 销毁完成
  activated() {} // 如果页面有keep-alive缓存功能，这个函数会触发
};
</script>

<style lang='less' scoped>
.contact-us {
  display: flex;
  align-items: center;
  flex-direction: column;
  justify-content: space-around;
}
@media screen and (min-width: 750px) {
  .contact-us {
    background-image: url('../static/pc/contact-us.png');
    background-size: 1920px 250px;
    width: 1920px;
    height: 250px;
    text-align: center;
    .contact-us-title {
      font-size: 45px;
      font-family: MicrosoftYaHei;
      color: #ffffff;
      line-height: 50px;
    }
    .contact-us-phone {
      font-size: 28px;
      text-align: center;
      font-family: MicrosoftYaHei;
      color: #ffffff;
      line-height: 60px;
      width: 280px;
      height: 60px;
      border: 2px solid #ffffff;
    }
  }
}
@media screen and (max-width: 750px) {
  .contact-us {
    background-image: url('../static/move/contact-us.png');
    background-size: 100vw 40vw;
    width: 100vw;
    height: 40vw;
    text-align: center;
  }
}
</style>