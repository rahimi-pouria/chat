<template>
  <div class="d-flex flex-column position-relative">
    <div class="d-flex w-100 p-5" style="background: #049686;"></div>
    <div
         class="d-flex w-100 h-100 align-items-center justify-content-center"
         style="background: #dfdfdf;height: 100vh">
      <div class="d-flex m-0 p-0 col-md-10 bg-white shadow-sm position-absolute" style="top: 65px">
        <BodyChat />
      </div>
    </div>
  </div>
</template>

<script>
import BodyChat from "../components/BodyChat";
export default {
  name: 'IndexPage',
  components: {BodyChat},
}
</script>
