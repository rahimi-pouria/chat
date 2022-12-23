<template>
  <div class="d-flex headerMessage p-2 justify-content-between align-items-center">
    <div class="d-flex align-items-center g8">
      <img src="@/assets/img/User.jpg" alt=""
           style="width: 50px; height: 50px; border-radius: 50%">
      <P>pouria rahimy</P>
    </div>
    <div class="d-flex g8">
            <span class="rounded-circle d-flex align-items-center pointer IconsHeader">
        <svg viewBox="0 0 24 24" height="24" width="24" preserveAspectRatio="xMidYMid meet"
             class="" version="1.1" x="0px" y="0px" enable-background="new 0 0 24 24"
             xml:space="preserve"><path fill="currentColor" d="M15.9,14.3H15L14.7,14c1-1.1,1.6-2.7,1.6-4.3c0-3.7-3-6.7-6.7-6.7S3,6,3,9.7 s3,6.7,6.7,6.7c1.6,0,3.2-0.6,4.3-1.6l0.3,0.3v0.8l5.1,5.1l1.5-1.5L15.9,14.3z M9.7,14.3c-2.6,0-4.6-2.1-4.6-4.6s2.1-4.6,4.6-4.6 s4.6,2.1,4.6,4.6S12.3,14.3,9.7,14.3z">

        </path></svg>
      </span>
      <span class="rounded-circle pointer d-flex align-items-center IconsHeader">
        <svg viewBox="0 0 24 24" height="24" width="24" preserveAspectRatio="xMidYMid meet"
             class="" version="1.1" x="0px" y="0px" enable-background="new 0 0 24 24" xml:space="preserve">
          <path fill="currentColor" d="M12,7c1.104,0,2-0.896,2-2c0-1.105-0.895-2-2-2c-1.104,0-2,0.894-2,2 C10,6.105,10.895,7,12,7z M12,9c-1.104,0-2,0.894-2,2c0,1.104,0.895,2,2,2c1.104,0,2-0.896,2-2C13.999,9.895,13.104,9,12,9z M12,15 c-1.104,0-2,0.894-2,2c0,1.104,0.895,2,2,2c1.104,0,2-0.896,2-2C13.999,15.894,13.104,15,12,15z"></path></svg>
      </span>
    </div>
  </div>
</template>

<script>
export default {
  name: "HeaderMessage"
}
</script>

<style scoped lang="scss">
.headerMessage {
  background: #f0f2f5;
  z-index: 9;
  position: absolute;
  top: 0;
  width: 100%;
}
</style>
