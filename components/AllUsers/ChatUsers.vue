<template>
  <div class="d-flex bg-white border flex-column" style="max-height: 88vh; overflow-y: scroll">
<!--    heaser chat-->
    <HeaderUserChat />
    <AllUsersShowUser />
  </div>
</template>

<script>
import HeaderUserChat from "./HeaderUserChat";
export default {
  name: "ChatUsers",
  components: {HeaderUserChat}
}
</script>

<style scoped>

</style>
