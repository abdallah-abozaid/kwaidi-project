<template>
  <div class="Section3">
    <div class="row">
      <div class="col-12 col-lg-7 d-flex align-items-center">
        <div>
          <h4 class="mb-3">
            ابدأ البيع معنا للوصول لاكثر من + مليون عميل يومياً
          </h4>
          <p class="desc mb-4">
            تأسست منصة كوايدي مول عام 2016 حيث تنوعت بخدمات ومزايا وتقنيات
            منافسة بين المنصات المحلية للانشطة التجارية والخدمية بجميع القطاعات
            التجزئة والجملة حيث يمكنك الوصول لعملائك بسهولة
          </p>
          <div class="cards my-5">
            <div class="row row-cols-1 row-cols-md-3 g-5">
              <div class="col">
                <div class="card">
                  <div class="card-body pb-2">
                    <h5 class="card-title download">
                      <span> 10</span><span class="mx-1">K</span>
                    </h5>
                    <p class="card-text">تحميلات.</p>
                  </div>
                </div>
              </div>
              <div class="col">
                <div class="card">
                  <div class="card-body pb-2">
                    <h5 class="card-title clints">
                      <span> 10</span><span class="mx-1">K</span>
                    </h5>
                    <p class="card-text">عملاء</p>
                  </div>
                </div>
              </div>
              <div class="col">
                <div class="card">
                  <div class="card-body pb-2">
                    <h5 class="card-title commits">
                      <span> 10</span><span class="mx-1">K</span>
                    </h5>
                    <p class="card-text">تعليقات ايجابية</p>
                  </div>
                </div>
              </div>
            </div>
          </div>
          <div class="featurs mb-5">
            <button class="mt-3">مزايا البيع معنا</button>
          </div>
          <div class="imgs">
            <img src="../../assets/home/googkeplay.png" alt="googkeplay" />
            <img src="../../assets/home/appStore.png" alt="appStore" />
          </div>
        </div>
      </div>
      <div class="col-12 col-lg-5 px-4">
        <img
          src="../../assets/home/Section3.png"
          alt="Section3"
          class="BigImg"
        />
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "HomeSection3",
  components: {},
};
</script>
<style lang="scss" scoped>
.Section3 {
  .BigImg {
    width: 100% !important;
  }
  margin-top: 50px;
}
h4 {
  color: rgba(95, 95, 95, 1);
  font-family: "DIN Next LT Arabic mediam", sans-serif;
}
.desc {
  font-size: 14px;
  color: rgba(95, 95, 95, 1);
  font-family: "DIN Next LT Arabic mediam", sans-serif;
}
.cards {
  width: 70%;
  text-align: center;

  .card {
    box-shadow: 0px 4px 50px 0px rgba(0, 0, 0, 0.05);
    border: none;
    border-radius: 20px;
    transition: all 0.3s linear;
    cursor: pointer;
    &:hover {
      transform: scale(1.1);
    }
    .card-title {
      display: flex;
      justify-content: center;
      align-items: center;
      color: #fff;
      height: 70px;
      width: 70px;
      margin: auto;
      margin-bottom: 10px;
      border-radius: 20px;
      font-size: 19px;
      direction: ltr;
    }
    .download {
      background: linear-gradient(
        321.45deg,
        #ff894b 13.54%,
        rgba(255, 137, 75, 0) 198.11%
      );
      filter: drop-shadow(0px 10px 10px rgba(255, 137, 75, 0.2));
    }
    .clints {
      background: linear-gradient(
        326.35deg,
        #d96d92 40.68%,
        rgba(217, 109, 146, 0) 146.75%
      );
      filter: drop-shadow(0px 10px 10px rgba(217, 109, 146, 0.2));
    }
    .commits {
      background: linear-gradient(
        325.27deg,
        #3fd2c2 7.21%,
        rgba(63, 210, 194, 0) 119.52%
      );
      filter: drop-shadow(0px 10px 10px rgba(58, 194, 203, 0.2));
    }
    .card-text {
      font-weight: 600;
      color: #5f5f5f;
      font-size: 12px;
    }
  }
}
.featurs button {
  background: #3ac2cb;
  border-radius: 9px;
  border: 1px solid #fff;
  padding: 12px;
  width: 250px;
  color: #fff;
  font-size: 18px;
  transition: all 0.3s linear;
  font-family: "DIN Next LT Arabic light", sans-serif;
  &:hover {
    background: #fff;
    border-radius: 9px;
    border: 1px solid #3ac2cb;
    color: #3ac2cb;
  }
}
.imgs {
  margin-top: 70px;
}
.imgs img {
  width: 160px;
  margin-left: 20px;
}
@media (max-width: 992px) {
  .cards {
    margin: auto;
  }
  .featurs {
    text-align: center;
  }
  .imgs {
    text-align: center;
  }
  .imgs img {
    width: 140px;
    margin-left: 10px;
  }
}
</style>
