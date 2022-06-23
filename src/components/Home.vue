<template>
  <header class="gradient-custom py-5">
    <div class="container px-4 px-lg-5 my-5">
      <div class="text-center text-white">
        <h1 class="display-2 fw-bolder">XeMart</h1>
        <p class="lead fw-normal text-white-50 mb-0">
          Hệ thống kinh doanh xe máy hàng đầu Việt Nam
        </p>
      </div>
    </div>
  </header>

  <Content />
</template>

<script>
import Content from "./Content.vue";
export default {
  name: "Home",
  components: {
    Content,
  },
};
</script>

<style>
.gradient-custom {
  /* fallback for old browsers */
  background: #6a11cb;

  /* Chrome 10-25, Safari 5.1-6 */
  background: -webkit-linear-gradient(
    to right,
    rgba(106, 17, 203, 1),
    rgba(37, 117, 252, 1)
  );

  /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */
  background: linear-gradient(
    to right,
    rgba(106, 17, 203, 1),
    rgba(37, 117, 252, 1)
  );
}
</style>