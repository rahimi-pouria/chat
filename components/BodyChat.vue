<template>
  <div class="d-flex w-100" style="height: 88vh">
    <div class="col-md-4 w-100 p-0 m-0">
      <AllUsersChatUsers />
    </div>
    <div class="col-md-8 w-100 p-0 m-0 position-relative">
      <AllMessagesHeaderMessage />
      <AllMessagesTypingMessage  class="position-absolute" style="bottom: 0"/>
    </div>
  </div>
</template>

<script>export default {
  name: "BodyChat",
  data () {
    return {
    }
  }
}
</script>

<style scoped lang="scss">
</style>
