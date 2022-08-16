<template>
  <div class="ProgramElement">
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
          <img src="../../assets/CartShoping/designing.png" alt="" />
        </div>
        <div class="flex">
          <div>
            <p class="title">تصميم تطبيق تجارة إلكترونية</p>
            <p class="subtitle">ملابس نسائية</p>
          </div>
          <div>
            <p class="title">مدة التنفيذ</p>
            <p class="newPrice">10 أيام</p>
          </div>
          <div>
            <p class="title">السعر</p>
            <p class="newPrice">100$</p>
          </div>
          <div>
            <p class="title">السعر الاجمالي</p>
            <p class="newPrice">100$</p>
          </div>
          <div class="deleteBTN">
            <button>
              <img src="../../assets/CartShoping/trash.png" alt="" />
            </button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "ProgramElement",
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
  padding-left: 0 !important;
  .form-check-input {
    margin-left: 15px;
    margin-top: 32px;
  }
}

.form-check-label {
  display: flex;
  width: 100%;
  .flex {
    display: flex;
    justify-content: space-between;
    width: 90%;
    padding-top: 18px;
  }
  & > div {
    margin: 0 10px;
  }
  & > div:first-of-type {
    margin-right: 0px;
  }
  & > div > img {
    width: 90px;
  }
  .title {
    font-size: 12px;
    font-weight: 600;
    margin-bottom: 10px;
    color: #5f5f5f !important;
  }
  .subtitle {
    font-size: 10px;
  }

  .newPrice {
    font-weight: 600;
    font-size: 12px;
    text-align: center;
  }
}
.deleteBTN button {
  background: transparent;
  border: none;
  img {
    width: 20px;
    margin-top: 20px;
  }
}
@media (max-width: 576px) {
  .form-check-label {
    background-color: #fff;
    margin-bottom: 20px;
    border-radius: 20px;
    padding: 10px;
    display: block;
    .flex {
      display: block;
      padding-top: 8px;
    }
    div {
      margin: 12 0px;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

    & > div > img {
      width: 70px;
    }
    .title {
      font-size: 13px;
      margin-bottom: 10px;
      color: #5f5f5f !important;
      font-family: "DIN Next LT Arabic bold", sans-serif;
    }
    .subtitle {
      font-size: 10px;
      margin: 0;
    }
    .oldPrice {
      margin-bottom: 0px;
      font-size: 12px;
      font-family: "DIN Next LT Arabic bold", sans-serif;
    }
    .newPrice {
      font-size: 11px;
      font-family: "DIN Next LT Arabic bold", sans-serif;
      margin-bottom: 0px;
    }
    .inputs {
      justify-content: center;
      margin-top: 0px;
      margin-bottom: 10px;
      input {
        width: 50px;
        font-size: 13px;
      }
    }
  }
  .deleteBTN {
    display: flex;
    justify-content: center !important;
  }
}
</style>
<style>
.form-check {
  padding: 0;
}
</style>
