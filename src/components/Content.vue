<template>
  <section class="py-5 position-relative">

  </section>
  <section class="py-5 position-relative">
    <div class="container px-4 px-lg-5">
      <div class="row gx-4 gx-lg-5 row-cols-2 row-cols-md-3 row-cols-xl-4 justify-content-center">
        <div class="col mb-5" v-for="item in items" :key="item.id">
          <router-link :to="{ name: 'Pdetail', params: { id: item.id } }">
            <div class="card h-100">
              <img class="card-img-top" :src="item.img" alt="..." />
              <div class="card-body p-2">
                <div class="text-center">
                  <div class="pull-left name-price">
                    <span class="fw-light fs-5">Duke 390</span>
                    <p>Đời 2022, Đã qua sử dụng</p>
                  </div>
                </div>
              </div>
              <div class="card-footer p-2 pt-0 border-top-0 bg-transparent">
                <div class="pull-left m-price">
                  <span class="fs-6 text-muted">59.000.000</span>
                </div>

                <div class="c-star">
                  <i class="bi bi-heart c-hart"></i>
                  <i class="bi bi-star-fill"></i><i class="bi bi-star-fill"></i
                  ><i class="bi bi-star-fill"></i><i class="bi bi-star-fill"></i
                  ><i class="bi bi-star-half"></i>
                </div>

                <div class="c-location fw-lighter">TP.Hồ Chí Minh</div>
              </div>
            </div>
          </router-link>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      items: [
        {
          id: "0",
          author: "PD 1",
          width: 200,
          height: 200,
          img: "https://chaumayman.com/wp-content/uploads/2021/11/KTM-Duke-200.png",
        },
        {
          id: "1",
          author: "PD 2",
          width: 200,
          height: 200,
          img: "https://chaumayman.com/wp-content/uploads/2021/11/KTM-Duke-200.png",
        },
        {
          id: "2",
          author: "PD 3",
          width: 200,
          height: 200,
          img: "https://chaumayman.com/wp-content/uploads/2021/11/KTM-Duke-200.png",
        },
        {
          id: "3",
          author: "PD 4",
          width: 200,
          height: 200,
          img: "https://chaumayman.com/wp-content/uploads/2021/11/KTM-Duke-200.png",
        },
        {
          id: "4",
          author: "PD 5",
          width: 200,
          height: 200,
          img: "https://chaumayman.com/wp-content/uploads/2021/11/KTM-Duke-200.png",
        },
        {
          id: "5",
          author: "PD 6",
          width: 200,
          height: 200,
          img: "https://chaumayman.com/wp-content/uploads/2021/11/KTM-Duke-200.png",
        },
        {
          id: "6",
          author: "PD 7",
          width: 200,
          height: 200,
          img: "https://chaumayman.com/wp-content/uploads/2021/11/KTM-Duke-200.png",
        },
        {
          id: "7",
          author: "PD 8",
          width: 200,
          height: 200,
          img: "https://chaumayman.com/wp-content/uploads/2021/11/KTM-Duke-200.png",
        },
        {
          id: "8",
          author: "PD 9",
          width: 200,
          height: 200,
          img: "https://chaumayman.com/wp-content/uploads/2021/11/KTM-Duke-200.png",
        },
        {
          id: "9",
          author: "PD 10",
          width: 200,
          height: 200,
          img: "https://chaumayman.com/wp-content/uploads/2021/11/KTM-Duke-200.png",
        },
        {
          id: "10",
          author: "PD 11",
          width: 200,
          height: 200,
          img: "https://chaumayman.com/wp-content/uploads/2021/11/KTM-Duke-200.png",
        },
        {
          id: "11",
          author: "PD 12",
          width: 200,
          height: 200,
          img: "https://chaumayman.com/wp-content/uploads/2021/11/KTM-Duke-200.png",
        },
      ],
    };
  },
};
</script>

<style scoped>
a {
  text-decoration: none;
}
.card {
  border-radius: 4px;
  background: #fff;
  box-shadow: 0 6px 10px rgba(0, 0, 0, 0.08), 0 0 6px rgba(0, 0, 0, 0.05);
  transition: 0.3s transform cubic-bezier(0.155, 1.105, 0.295, 1.12),
    0.3s box-shadow,
    0.3s -webkit-transform cubic-bezier(0.155, 1.105, 0.295, 1.12);
  cursor: pointer;
}

.card:hover {
  transform: scale(1.03);
  box-shadow: 0 10px 20px rgba(0, 0, 0, 0.12), 0 4px 8px rgba(0, 0, 0, 0.06);
}
.m-price {
  white-space: nowrap;
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