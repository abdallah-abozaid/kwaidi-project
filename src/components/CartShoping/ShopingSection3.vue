<template>
  <div class="ShopingSection3">
    <div class="form-check mb-3">
      <input
        class="form-check-input"
        type="checkbox"
        value=""
        id="flexCheckChecked"
        checked
      />
      <label class="form-check-label" for="flexCheckChecked">
        تحديد الكل
      </label>
    </div>

    <div class="row row-cols-1 row-cols-lg-2 g-4">
      <div class="col-12 col-lg-8">
        <div class="card mb-4">
          <div class="card-body">
            <ClothesCart />
          </div>
        </div>
        <div class="card mb-4">
          <div class="card-body">
            <ProgrammingCart />
          </div>
        </div>
        <div class="card mb-4">
          <div class="card-body">
            <MicrsoftCart />
          </div>
        </div>
        <div class="card mb-4">
          <div class="card-body">
            <DonationCart />
          </div>
        </div>
      </div>
      <div class="col-12 col-lg-4 mb-4">
        <div class="card">
          <div class="card-body">
            <OrderSammary />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import OrderSammary from "./OrderSammary.vue";
import ClothesCart from "./ClothesCart.vue";
import ProgrammingCart from "./ProgrammingCart.vue";
import MicrsoftCart from "./MicrsoftCart.vue";
import DonationCart from "./DonationCart.vue";
export default {
  name: "ShopingSection3",
  components: {
    OrderSammary,
    ClothesCart,
    ProgrammingCart,
    MicrsoftCart,
    DonationCart,
  },
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
    margin-left: 10px;
  }
  label {
    font-size: 17px;
    display: flex;
    align-items: flex-end;
  }
}
.card {
  border: none;
  background: #fafafa;
  border-radius: 20px;
}
</style>
