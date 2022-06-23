<template>
  <div>
    <nav class="navbar navbar-expand-lg navbar-light gradient-custom">
      <div class="container px-4 px-lg-5">
        <router-link class="navbar-brand text-white" to="/">XeMart</router-link>

        <button
          class="navbar-toggler"
          type="button"
          data-bs-toggle="collapse"
          data-bs-target="#navbarSupportedContent"
          aria-controls="navbarSupportedContent"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarSupportedContent">
          <ul class="navbar-nav me-auto mb-2 mb-lg-0 ms-lg-4">
            <li class="nav-item">
              <router-link class="nav-link active text-white" to="/"
                >Trang chủ</router-link
              >
            </li>
            <li class="nav-item">
              <a class="nav-link text-white" href="/Login">Đăng nhập</a>
            </li>
            <li class="nav-item dropdown">
              <a
                class="nav-link dropdown-toggle text-white"
                id="navbarDropdown"
                href="#"
                role="button"
                data-bs-toggle="dropdown"
                aria-expanded="false"
                >Sản phẩm</a
              >
              <ul class="dropdown-menu" aria-labelledby="navbarDropdown">
                <li><a class="dropdown-item" href="#!">Tất cả sản phẩm</a></li>
                <li><hr class="dropdown-divider" /></li>
                <li><a class="dropdown-item" href="#!">Xe số</a></li>
                <li><a class="dropdown-item" href="#!">Xe tay ga</a></li>
                <li><a class="dropdown-item" href="#!">Xe phân khối lớn</a></li>
                <li><a class="dropdown-item" href="#!">Xe điện</a></li>
              </ul>
            </li>
          </ul>
          <form class="d-flex">
            <input
              class="form-control mr-sm-5"
              type="search"
              placeholder="Tìm kiếm"
              aria-label="Search"
            />
            <button type="button" class="btn btn-dark mx-lg-2"><i class="bi bi-search"></i></button>
          </form>
          <form class="d-flex">
            <button class="btn btn-outline-danger text-white" type="submit">
              <i class="bi-cart-fill me-1"></i>
              Giỏ hàng
              <span class="badge bg-dark text-white ms-1 rounded-pill">0</span>
            </button>
          </form>
        </div>
      </div>
    </nav>
  </div>
</template>

<script>
export default {};
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
