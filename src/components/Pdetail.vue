<template>
  <section class="py-5">
    <div class="container px-4 px-lg-5">
      <h1>Chi tiết sản phẩm</h1>

      <div class="card mb-3 border-0">
        <div class="row g-0">
          <div class="col-md-4">
            <img
              style="margin-bottom: 0.3rem"
              src="/src/assets/duke800800.png"
              class="img-fluid rounded-start"
              alt="..."
            />
            <div>
              <img
                src="/src/assets/duke120120.jpg"
                alt=""
                style="margin-left: 0.7rem"
              />
              <img
                src="/src/assets/duke120120.jpg"
                alt=""
                style="margin-left: 0.7rem"
              />
              <img
                src="/src/assets/duke120120.jpg"
                alt=""
                style="margin-left: 0.7rem"
              />
            </div>
          </div>
          <div class="col-md-8">
            <div class="card-body">
              <h3 class="card-title">DUKE 390</h3>
              <div class="mb-1">
                <div class="pull-left m-price">
                  <span class="fs-4 s-price">59.000.000</span>
                </div>

                <div class="c-star">
                  <i class="bi bi-star-fill"></i><i class="bi bi-star-fill"></i
                  ><i class="bi bi-star-fill"></i><i class="bi bi-star-fill"></i
                  ><i class="bi bi-star-half"></i>
                </div>
                <p>30 xe đã bán</p>
              </div>
              <p class="card-text">
                Ktm duke 390 2020 abs - Xe dàn ngoài đẹp keng, ốc tán zin đẹp +
                Xe lên Pô arrow real ( 7tr5 ) + Khung chống đổ + Kính gù Đồ zin
                còn đủ - xe máy móc bảo dưỡng đầy đủ hãng , bao zin, mạnh êm ,
                odo chuẩn 11k - Xe bs tỉnh 60 , chính chủ, sang tên nhanh chóng,
                hỗ trợ ae rút gốc nếu cần Giá fix nhẹ ưu tiên ae xem xe trực
                tiếp Xem xe hcm q6 Nhận gl xe khác #ktm #duke390
              </p>
              <button type="button" class="btn btn-primary">
                <i class="bi bi-cart4"></i> Đặt hàng ngay
              </button>
              <button type="button" class="btn btn-warning ms-lg-2">
                <i class="bi bi-telephone-fill"></i> Liên hệ
              </button>
              <p class="card-text">
                <small class="text-muted"
                  >Lần cuối cập nhật: 35 phút trước.</small
                >
              </p>
            </div>
          </div>
        </div>
      </div>
      <br />
      <hr />
      <div class="card border-0">
        <div class="card-body">
          <h4 class="card-title">Các sản phẩm tương tự</h4>
          <Content />
        </div>
      </div>
      <br />
      <br />
    </div>
  </section>
</template>

<script>
import Content from "./Content.vue";
export default {
  data() {
    return {
      id: this.$route.params.id,
    };
  },
  components: {
    Content,
  },
};
</script>

<style scoped>
.m-price {
  white-space: nowrap;
}

.m-price .s-price {
  color: brown;
  padding-bottom: 1rem;
}
.name-price {
  text-align: left;
  padding-bottom: 2rem;
}
.c-hart {
  color: darkgray;
  padding: 0.5rem;
}
.c-star {
  color: orange;
  padding-top: 0.5rem;
}
.c-location {
  text-align: right;
  color: darkgrey;
  padding-top: 0.5rem;
}
</style>
