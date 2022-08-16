<template>
  <div class="ClothesCart">
    <div class="form-check">
      <input
        class="form-check-input"
        type="checkbox"
        value=""
        id="flexCheckChecked"
        checked
      />
      <div class="form-check-label" for="flexCheckChecked">
        <div>
          <div class="Store mb-2">
            <img src="../../assets/CartShoping/zara.png" alt="" />
            <p>متجر زارا -Zara Store</p>
          </div>
          <div>
            <p class="red">
              هذا المتجر يتطلب الشراء بمبلغ لايقل عن 100 ريال لاتمام الطلب
            </p>
          </div>
        </div>
      </div>
    </div>
    <hr class="mt-0" />
    <OrderElement />
    <OrderElement />
    <hr />
    <div class="row">
      <div class="col-12 col-md-8">
        <div class="inner pe-0 pe-md-5">
          <div class="dropdown mb-3">
            <button
              class="btn dropdown-toggle"
              type="button"
              data-bs-toggle="dropdown"
              aria-expanded="false"
            >
              وسيلة الشحن
            </button>
            <ul class="dropdown-menu">
              <li>
                <div>
                  <img src="../../assets/CartShoping/knagr.png" alt="" />
                </div>
                <div class="texts">
                  <h6 class="mb-1">شركة Knagr للتوصيل السريع</h6>
                  <p class="mb-1">سعر الشحن 10$</p>
                  <p class="mb-1">الوقت المتوقع للتوصيل : 1-3 ساعات</p>
                </div>
              </li>
              <li>
                <div>
                  <img src="../../assets/CartShoping/smsa.png" alt="" />
                </div>
                <div class="texts">
                  <h6 class="mb-1">شركة smsa للتوصيل السريع</h6>
                  <p class="mb-1">سعر الشحن 10$</p>
                  <p class="mb-1">الوقت المتوقع للتوصيل : 1-3 ساعات</p>
                </div>
              </li>
              <li>
                <div>
                  <img src="../../assets/CartShoping/group.png" alt="" />
                </div>
                <div class="texts">
                  <h6 class="mb-1">سيتم التوصيل من خلال التاجر</h6>
                  <p class="mb-1">سعر الشحن مجاني</p>
                  <p class="mb-1">
                    الوقت المتوقع للتوصيل : حسب المتفق عليه أو فوري
                  </p>
                </div>
              </li>
              <li>
                <div>
                  <img src="../../assets/CartShoping/shop.png" alt="" />
                </div>
                <div class="texts">
                  <h6 class="mb-1">استلام من الفرع</h6>
                </div>
              </li>
            </ul>
          </div>
          <div class="flexing">
            <div class="inputCode">
              <input type="text" value="123456" />
              <img src="../../assets/CartShoping/tick-circle.png" alt="" />
            </div>
            <div>
              <button>تطبيق</button>
            </div>
          </div>
        </div>
      </div>
      <div class="col-12 col-md-4 last">
        <div>
          <p>القيمة الفرعية للمتجر</p>
          <p>600$</p>
        </div>
        <div>
          <p>القيمة المضافة</p>
          <p>10$</p>
        </div>
        <div>
          <p>قيمة الشحن</p>
          <p>10$</p>
        </div>
        <div>
          <p>الإجمالي</p>
          <p class="color">620$</p>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import OrderElement from "./OrderElement.vue";
export default {
  name: "ClothesCart",
  components: { OrderElement },
};
</script>
<style lang="scss" scoped>
.form-check-input:checked {
  background-color: rgba(58, 194, 203, 1);
  border-color: rgba(58, 194, 203, 1);
}
.form-check-input {
  width: 1.5rem;
  height: 1.5rem;
}
.form-check {
  display: flex;
  .form-check-input {
    margin-left: 15px;
    margin-top: 10px;
  }
}
hr {
  border-color: #d9d9d9;
}
.Store {
  display: flex;
  align-items: center;
  img {
    width: 40px;
  }
  p {
    margin: 0 10px;
    font-family: "DIN Next LT Arabic bold", sans-serif;
    color: #5f5f5f;
    font-size: 13px;
  }
}
.red {
  font-size: 10px;
  font-weight: 500;
  color: #cd1717;
}
.dropdown-toggle {
  background-color: #fff !important;
  width: 100%;
  text-align: right;
  position: relative;
  border-radius: 20px;
  border: 1px solid rgba(234, 234, 234, 1);
  color: #5f5f5f;
  font-size: 12px;
  &::after {
    position: absolute;
    top: 50%;
    left: 10px;
  }
}
.inner {
  width: 70%;
}
.flexing {
  display: flex;
  justify-content: space-between;
  align-items: center;
  button {
    background-color: rgba(58, 194, 203, 1);
    border: none;
    color: #fff;
    width: 70px;
    border-radius: 20px;
    font-size: 12px;
    padding: 6px;
  }
}
.inputCode {
  width: 100%;
  position: relative;

  img {
    position: absolute;
    top: 50%;
    right: 65%;
    transform: translateY(-50%);
    width: 20px;
  }
  input {
    width: 85%;
    border-radius: 20px;
    border: 1px solid rgba(58, 194, 203, 1);
    padding: 7px;
    font-size: 12px;
    color: #5f5f5f;
    background: #edfafb;
    &::placeholder {
      font-size: 12px;
      color: #9a9a9a;
    }
  }
}
.last div {
  display: flex;
  align-items: center;
  justify-content: space-between;
  font-family: "DIN Next LT Arabic bold", sans-serif;
  font-size: 13px;
  p:first-of-type {
    color: #5f5f5f;
  }
  .color {
    color: #3ac2cb;
  }
}
.dropdown-menu {
  background-color: #fafafa;
  border-radius: 20px;
  width: 100%;
  border-color: rgb(243, 243, 243);
  li {
    display: flex;
    justify-content: flex-start;
    text-align: right;
    padding: 10px;
    border-bottom: 1px solid #e2e2e2;
    cursor: pointer;
    & > div:first-of-type {
      width: 25%;
      display: flex;
      align-items: flex-start;
      justify-content: center;
    }
    &:last-of-type {
      border: none;
      padding-top: 20px;
      padding-bottom: 0px;
    }

    .texts p {
      font-size: 10px;
      color: #9a9a9a;
    }
    .texts h6 {
      font-size: 12px;
    }
  }
}
</style>
