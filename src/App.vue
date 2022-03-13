<template>
  <div class="app">
    <FriendList/>
    <ContactUs />
  </div>
</template>

<script>
import FriendList from "./component/friend-list.vue"
import ContactUs from './component/contact-us.vue';
export default {
  name: 'App',
  components: {
    FriendList,
    ContactUs
  }
};
</script>

<style>
* {
  padding: 0px;
  margin: 0px;
}
.app {
  width: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
  overflow-x: hidden;
}
</style>
