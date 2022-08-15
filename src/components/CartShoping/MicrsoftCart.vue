<template>
  <div class="MicrosoftCart">
    <div class="form-check mb-3">
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
            <img src="../../assets/CartShoping/micrsoft.png" alt="" />
            <p>شركة مايكروسوفت</p>
          </div>
        </div>
      </div>
    </div>
    <OfficeElement />
    <div>
      <div class="inner pe-0 pe-md-5">
        <div class="options">
          <p class="title mt-4">خيارات</p>
          <div class="d-flex align-items-center">
            <div class="dropdown">
              <button
                class="btn dropdown-toggle"
                type="button"
                data-bs-toggle="dropdown"
                aria-expanded="false"
              >
                سنة واحدة
              </button>
              <ul class="dropdown-menu">
                <li>
                  <a href="/">سنة واحدة</a>
                </li>
                <li>
                  <a href="/">سنة واحدة</a>
                </li>
                <li>
                  <a href="/">سنة واحدة</a>
                </li>
              </ul>
            </div>
            <div class="dropdown">
              <button
                class="btn dropdown-toggle"
                type="button"
                data-bs-toggle="dropdown"
                aria-expanded="false"
              >
                النسخة الاحترافية
              </button>
              <ul class="dropdown-menu">
                <li>
                  <a href="/">النسخة الاحترافية</a>
                </li>
                <li>
                  <a href="/">النسخة الاحترافية</a>
                </li>
                <li>
                  <a href="/">النسخة الاحترافية</a>
                </li>
              </ul>
            </div>
          </div>
          <p class="title my-3">
            سيتم ارسال الكود الى ايميلك وايضاً يمكنك نسخ البيانات من تفاصيل
            الطلب بعد الدفع
          </p>
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
  </div>
</template>
<script>
import OfficeElement from "./OfficeElement.vue";
export default {
  name: "MicrosoftCart",
  components: { OfficeElement },
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
    font-weight: 600;
    color: #5f5f5f;
    font-size: 13px;
  }
}
.title {
  font-weight: 600;
  margin-bottom: 10px;
  font-size: 12px;
}
.dropdown {
  width: 150px;
  margin-left: 20px;
}
.dropdown-toggle {
  background-color: #fff !important;
  width: 100%;
  text-align: right;
  position: relative;
  border-radius: 10px;
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
  width: 100%;
}
.flexing {
  display: flex;
  align-items: center;
  button {
    background-color: rgba(58, 194, 203, 1);
    border: none;
    color: #fff;
    width: 70px;
    border-radius: 20px;
    padding: 6px;
    font-size: 12px;
  }
}
.inputCode {
  position: relative;
  margin-left: 10px;
  input {
    width: 150px;
    border-radius: 20px;
    border: 1px solid rgba(234, 234, 234, 1);
    padding: 7px;
    font-size: 11px;
    color: #5f5f5f;
    &::placeholder {
      font-size: 11px;
      color: #9a9a9a;
    }
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
      font-size: 11px;
      color: #9a9a9a;
    }
    .texts h6 {
      font-size: 13px;
    }
  }
}
</style>
