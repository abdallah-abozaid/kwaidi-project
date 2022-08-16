<template>
  <div class="ShopingSection2 mb-5">
    <div class="outer">
      <div class="form-check form-switch">
        <label class="switch">
          <input type="checkbox" checked />
          <span class="slider round"></span>
        </label>
      </div>
    </div>
    <h5 class="mb-4">عربة التسوق</h5>
    <div class="cards mt-3">
      <div class="row row-cols-1 row-cols-md-2 gx-5 gy-2">
        <div class="col">
          <div class="card">
            <div class="card-body">
              <div>
                <div class="title mb-3">
                  <img src="../../assets/CartShoping/location.png" alt="" />
                  <p class="mb-0 mx-2">عنوان التوصيل</p>
                </div>
                <p class="desc mb-0">2091 الملك سعود , الفيحاء الدمام</p>
              </div>
              <div>
                <button>تغيير</button>
              </div>
            </div>
          </div>
        </div>
        <div class="col">
          <div class="card">
            <div class="card-body">
              <div>
                <div class="title mb-3">
                  <img src="../../assets/CartShoping/location.png" alt="" />
                  <p class="mb-0 mx-2">الفاتورة الضريبية</p>
                </div>
                <p class="desc mb-0">أحمد محمد</p>
              </div>
              <div>
                <button>تغيير</button>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "ShopingSection2",
};
</script>
<style lang="scss" scoped>
h5 {
  font-family: "DIN Next LT Arabic mediam", sans-serif;
}
.card {
  border: 2px solid rgba(217, 217, 217, 1);
  border-radius: 20px;
  .card-body {
    display: flex;
    justify-content: space-between;
    align-items: center;
    .title {
      display: flex;
      justify-content: flex-start;
      align-items: center;
      font-size: 14px;
      img {
        width: 19px;
      }
      p {
        font-weight: 500;
        color: #5f5f5f;
      }
    }
    .desc {
      font-size: 15px;
      color: #353535;
      font-weight: 500;
    }
  }
  button {
    padding: 10px;
    width: 130px;
    background: #fafafa;
    border-radius: 10px;
    border: none;
    font-size: 15px;
    font-family: "DIN Next LT Arabic bold", sans-serif;
    color: #3ac2cb;
  }
}
// switch ------------------------
.ShopingSection2 {
  position: relative;
}
.ShopingSection2 .outer {
  position: absolute;
  bottom: -10%;
  right: -11%;
}

.form-switch {
  transform: rotate(-90deg);
}
.switch {
  position: relative;
  display: inline-block;
  width: 125px;
  height: 40px;
}

.switch input {
  opacity: 0;
  width: 0;
  height: 0;
}

.slider {
  position: absolute;
  cursor: pointer;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background-color: #fafafa;
  -webkit-transition: 0.4s;
  transition: 0.4s;
}

.slider:before {
  position: absolute;
  content: "مظلم";
  height: 30px;
  width: 60px;
  left: 4px;
  bottom: 4px;
  background-color: white;
  -webkit-transition: 0.4s;
  transition: 0.4s;
  display: flex;
  align-items: center;
  font-weight: 700;
  justify-content: center;
  border: 1px solid #ccc;
  font-size: 12px;
}

input:checked + .slider {
  background-color: #5f5f5f;
}
input:checked + .slider::before {
  content: "مضيئ";
}

input:focus + .slider {
  box-shadow: 0 0 1px #5f5f5f;
}

input:checked + .slider:before {
  -webkit-transform: translateX(54px);
  -ms-transform: translateX(54px);
  transform: translateX(54px);
}

/* Rounded sliders */
.slider.round {
  border-radius: 34px;
  border: 1px solid #ccc;
}

.slider.round:before {
  border-radius: 30px;
}
// responsive

@media (max-width: 992px) {
  .fst {
    padding: 0px 4%;
    margin-bottom: 13px;
  }
  .sec {
    padding: 0px 4%;
  }
  .fst img:first-of-type {
    margin-left: 14px;
  }
  .fst img:last-of-type {
    width: calc(70% - 14px);
  }
  .sec img {
    margin-bottom: 13px;
  }
  .sec img:nth-of-type(1),
  .sec img:nth-of-type(3) {
    margin-left: 3%;
  }
  .ShopingSection2 .outer {
    right: -20%;
  }
  .ShopingSection2 .outer {
    display: none;
  }
}
</style>
