<template>
  <div>
    <!-- Footer-->
    <footer class="py-3 gradient-custom">
      <div class="container">
        <p class="m-0 text-center text-white">
          Copyright &copy; LTTC {{ year }}
        </p>
      </div>
    </footer>
  </div>
</template>

<script>
import { computed } from "@vue/reactivity";
export default {
  setup() {
    const year = computed(() => new Date().getFullYear());
    return { year };
  },
};
</script>

<style>
.gradient-custom {
/* fallback for old browsers */
background: #6a11cb;

/* Chrome 10-25, Safari 5.1-6 */
background: -webkit-linear-gradient(to right, rgba(106, 17, 203, 1), rgba(37, 117, 252, 1));

/* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */
background: linear-gradient(to right, rgba(106, 17, 203, 1), rgba(37, 117, 252, 1))
}
</style>