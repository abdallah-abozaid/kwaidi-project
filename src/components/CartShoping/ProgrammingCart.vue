<template>
  <div class="ProgrammingCart">
    <div class="form-check">
      <input
        class="form-check-input"
        type="checkbox"
        value=""
        id="flexCheckChecked"
        checked
      />
      <div class="form-check-label w-100 mb-2" for="flexCheckChecked">
        <div class="d-flex justify-content-between align-items-center">
          <div class="Store mb-2">
            <img src="../../assets/CartShoping/programming.png" alt="" />
            <p>شركة الخطوط للبرمجة والتسويق</p>
          </div>
          <div>
            <a href="/"
              ><img src="../../assets/CartShoping/tabby.png" alt=""
            /></a>
          </div>
        </div>
      </div>
    </div>
    <hr class="mt-0" />
    <ProgramElement />
    <hr />
    <div class="row">
      <div class="col-12 col-md-8">
        <div class="inner pe-0 pe-md-5">
          <button class="mb-2">
            <img src="../../assets/CartShoping/export.png" alt="" />
            <span>رفع الملفات </span>
          </button>
          <div class="constrain">
            <p>أقصى حجم للملفات 500 ميجابايت</p>
            <p>الصيغ المسموح : tpng ,jpg,zip,rar,pdf,word,ppt</p>
            <p class="mt-2">
              <img src="../../assets/CartShoping/add.png" alt="" />filename.pdf
            </p>
            <p class="red my-2">
              سيتم حذف الملفات اتوماتيكياً خلال 30 يوم من رفعها بالسلة
            </p>
            <p class="addNote">إضافة ملاحظات</p>
            <textarea
              class="mb-3"
              placeholder="من فضلك اكتب ملاحظاتك على الطلب هنا"
            ></textarea>
          </div>
          <div class="flexing">
            <div class="inputCode">
              <input type="text" placeholder="كوبون المتجر" />
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
import ProgramElement from "./ProgramElement.vue";
export default {
  name: "ProgrammingCart",
  components: { ProgramElement },
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
.d-flex img {
  width: 80px;
}
.Store {
  display: flex;
  align-items: center;
  img {
    width: 40px;
  }
  p {
    margin: 0 10px;
    font-weight: 600;
    color: #5f5f5f;
    font-size: 13px;
  }
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
  & > button {
    background-color: rgba(58, 194, 203, 1);
    border: none;
    color: #fff;
    width: 130px;
    border-radius: 20px;
    padding: 6px;
    img {
      margin: 0 0 0 5px;
      width: 16px;
      height: 16px;
    }
  }
}
.flexing {
  display: flex;
  justify-content: space-between;
  align-items: center;
  button {
    background-color: rgba(58, 194, 203, 1);
    border: none;
    color: #fff;
    width: 100px;
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
    width: 90%;
    border-radius: 20px;
    border: 1px solid rgba(234, 234, 234, 1);
    padding: 7px;
    font-size: 12px;
    color: #5f5f5f;
    &::placeholder {
      font-size: 11px;
      color: #9a9a9a;
    }
  }
}
.last div {
  display: flex;
  align-items: center;
  justify-content: space-between;
  font-weight: 600;
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
      font-size: 12px;
      color: #9a9a9a;
    }
    .texts h6 {
      font-size: 15px;
    }
  }
}
.constrain {
  p {
    font-size: 12px;
    color: #5f5f5f;
    margin-top: 4px;
    margin-bottom: 0px;
    & > img {
      transform: rotate(-45deg);
    }
  }
  .red {
    color: rgba(205, 23, 23, 1);
    font-size: 10px;
  }
  .addNote {
    font-size: 13px;
    font-weight: 600;
    margin-bottom: 10px;
  }
  textarea {
    background: #ffffff;
    border: 1px solid #eaeaea;
    border-radius: 15px;
    width: 100%;
    padding: 10px;
    height: 100px;
    font-size: 11px;
    &::placeholder {
      font-size: 11px;
      color: #9a9a9a;
    }
  }
}
@media (max-width: 576px) {
  .inner {
    width: 100%;
  }
}
</style>
