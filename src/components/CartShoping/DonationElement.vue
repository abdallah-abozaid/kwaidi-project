<template>
  <div class="DonationElement mb-4">
    <div class="form-check">
      <input
        class="form-check-input"
        type="checkbox"
        value=""
        id="flexCheckChecked"
        checked
      />
      <div class="form-check-label" for="flexCheckChecked">
        <div class="cart">
          <img src="../../assets/CartShoping/DonationtCart.png" alt="" />
        </div>
        <div class="flex">
          <div>
            <p class="title">تبرع لأغراض خيرية</p>
          </div>
          <div>
            <nav class="d-flex align-items-center p-0">
              <ul class="pagination p-0 m-0">
                <li class="page-item"><a class="page-link" href="#">1</a></li>
                <li class="page-item active" aria-current="page">
                  <a class="page-link" href="#">2</a>
                </li>
                <li class="page-item"><a class="page-link" href="#">3</a></li>
              </ul>
              <input type="text" placeholder="مبلغ آخر" />
            </nav>
          </div>
          <div class="pt-3">
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
  name: "DonationElement",
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
    align-items: center;
    width: 90%;
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
    font-size: 13px;
    margin-bottom: 10px;
    color: #5f5f5f !important;
    font-family: "DIN Next LT Arabic bold", sans-serif;
  }
  .newPrice {
    font-weight: 600;
    font-size: 12px;
    text-align: center;
  }
  .cart {
    display: flex;
    align-items: center;
    justify-content: center;
    background-color: white;
    width: 90px;
    padding: 20px 10px;
    border-radius: 16px;
    img {
      width: 45px;
    }
  }
}
.deleteBTN button {
  background: transparent;
  border: none;
  img {
    width: 20px;
  }
}
.pagination li {
}
.pagination li a {
  border-radius: 50% !important;
  margin: 0 5px !important;
  color: #5f5f5f;
  border: 1px solid #eaeaea;
  width: 40px;
  height: 40px;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 12px;
}
.pagination li.active a {
  background-color: #3ac2cb;
  color: #fff;
  border: 1px solid #3ac2cb;
}
nav input {
  width: 100px;
  background: #ffffff;
  border: 1px solid #eaeaea;
  border-radius: 25px;
  padding: 7px 10px;
  font-size: 11px;
  &::placeholder {
    color: #e6e6e6;
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
      margin-bottom: 5px;
      font-family: "DIN Next LT Arabic bold", sans-serif;
    }
    .subtitle {
      font-size: 10px;
    }
    .oldPrice {
      margin-bottom: 0px;
      font-size: 12px;
      font-family: "DIN Next LT Arabic bold", sans-serif;
    }
    .newPrice {
      font-size: 11px;
      margin-bottom: 0px;
      font-family: "DIN Next LT Arabic bold", sans-serif;
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
