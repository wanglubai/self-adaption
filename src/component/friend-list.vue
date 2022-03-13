<template>
  <div class="friend-list">
    <div class="friend-list-title">合作伙伴</div>
    <div class="friend-list-items">
      <div
        v-for="(item, i) in 18"
        :key="i"
        :class="['friend-list-item', 'friend-list-item' + (i + 1)]"
      ></div>
    </div>
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
@media screen and (min-width: 750px) {
  .friend-list-items {
    display: flex;
    flex-wrap: wrap;
    width: 1200px;
    justify-content: space-between;
  }
}
@media screen and (max-width: 750px) {
  .friend-list-items {
    display: flex;
    flex-wrap: wrap;
    width: 100vw;
    justify-content: space-around;
  }
}
.friend-list {
  text-align: center;
  padding-bottom: 60px;
}
.friend-list-title {
  font-size: 28px;
  font-family: MicrosoftYaHei;
  color: #333333;
  line-height: 37px;
}

.friend-list-item {
  width: 180px;
  height: 80px;
  margin-top: 24px;

  .loop(@i) when (@i <=18) {
    .loop((@i + 1));
    &:nth-child(@{i}) {
      background-image: url('../static/common/friend/lg@{i}.png');
    }
  }
  .loop(1);
}
</style>