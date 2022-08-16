<template>
  <div class="ShopingSection1">
    <nav aria-label="breadcrumb" class="p-2 px-0">
      <ol class="breadcrumb">
        <li class="breadcrumb-item">
          <router-link to="/">الرئيسية</router-link>
        </li>
        <li class="breadcrumb-item active" aria-current="page">عربة التسوق</li>
      </ol>
    </nav>
  </div>
</template>
<script>
export default {
  name: "ShopingSection1",
};
</script>
<style lang="scss" scoped>
.breadcrumb {
  font-size: 12px;
}
.breadcrumb-item:first-of-type {
  font-family: "DIN Next LT Arabic light", sans-serif;
}
.breadcrumb-item:last-of-type {
  color: #9a9a9a;
}
.breadcrumb-item + .breadcrumb-item::before {
  float: right;
}
.breadcrumb-item + .breadcrumb-item::before {
  content: url(../../assets/CartShoping/arrow-left.png);
}
.breadcrumb-item + .breadcrumb-item::before {
  padding-right: 0px;
}
</style>
