<template>
  <div class="OrderSammary py-2">
    <h4>ملخص اجمالي الطلب</h4>
    <hr class="mt-1 mb-4" />
    <div class="d-flex">
      <p>عدد المتاجر المختارة :</p>
      <p class="mx-2">2</p>
    </div>
    <div class="d-flex justify-content-between">
      <p>عدد العناصر 2</p>
      <p>500$</p>
    </div>
    <div class="d-flex justify-content-between">
      <p>اجمالي سعر الشحن</p>
      <p>10$</p>
    </div>
    <div class="d-flex justify-content-between">
      <p>قيمة الضريبة المضافة</p>
      <p>10$</p>
    </div>
    <div class="d-flex justify-content-between mb-3">
      <p>إجمالي خصومات الكوبونات</p>
      <p>50$</p>
    </div>
    <div class="d-flex mb-3">
      <p>الفاتورة الضريبية :</p>
      <p class="mx-2">أحمد محمد</p>
    </div>
    <p class="mb-1">عنوان التوصيل</p>
    <div class="d-flex mb-2">
      <div class="location d-flex justify-content-between">
        <p>السعودية , الدمام</p>
        <img src="../../assets/CartShoping/location.png" alt="" />
      </div>
    </div>
    <br />
    <p class="mb-1">كود خصم اضافي من كوايدي</p>
    <div class="code d-flex justify-content-between">
      <div class="inputCode">
        <input type="text" placeholder="قم بإدخال الكوبون الخاص بك" />
        <img src="../../assets/CartShoping/tick-circle.png" alt="" />
      </div>
      <div>
        <button>تطبيق</button>
      </div>
    </div>
    <hr class="my-4" />
    <div class="total d-flex justify-content-between">
      <p>الاجمالي شامل القيمة المضافة</p>
      <p class="Bold">510$</p>
    </div>
    <button class="pay">ادفع الآن</button>
  </div>
</template>
<script>
export default {
  name: "OrderSammary",
};
</script>
<style lang="scss" scoped>
hr {
  border-color: #d9d9d9;
}
p {
  font-size: 16px;
  color: #5f5f5f;
  margin-bottom: 11px;
  font-family: "DIN Next LT Arabic mediam", sans-serif;
}
.d-flex.justify-content-between > p:last-of-type {
  font-family: "DIN Next LT Arabic mediam", sans-serif;
}
.location {
  background: #fff;
  border-radius: 20px;
  border: 1px solid #eaeaea;
  width: 100%;
  align-items: center;
  padding: 7px;
  p {
    transform: translateY(2px);
    font-size: 11px;
    margin: 0;
    color: #353535;
    margin-right: 4px;
  }
}
.code {
  .inputCode {
    position: relative;
    img {
      position: absolute;
      top: 50%;
      right: 65%;
      transform: translateY(-50%);
      width: 20px;
    }
    input {
      width: 80%;
      border-radius: 20px;
      border: 1px solid rgba(234, 234, 234, 1);
      padding: 7px;
      &::placeholder {
        font-size: 10px;
        color: #9a9a9a;
      }
    }
  }
  button {
    background: #3ac2cb;
    border-radius: 25px;
    border: none;
    color: #fff;
    padding: 7px;
    width: 100px;
    font-size: 12px;
  }
}
.total {
  p {
    font-family: "DIN Next LT Arabic bold", sans-serif;
    font-size: 13px;
    &:last-of-type {
      color: #3ac2cb;
    }
  }
}
button.pay {
  width: 100%;
  background: #3ac2cb;
  border-radius: 25px;
  border: none;
  color: #fff;
  padding: 7px;
  margin-top: 10px;
  font-size: 13px;
}
</style>
