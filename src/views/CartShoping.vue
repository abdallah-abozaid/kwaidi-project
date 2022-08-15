<template>
  <div class="CartShoping container">
    <ShopingSection1 />
    <ShopingSection2 />
    <ShopingSection3 />
  </div>
</template>
<script>
import ShopingSection1 from "@/components/CartShoping/ShopingSection1.vue";
import ShopingSection2 from "@/components/CartShoping/ShopingSection2.vue";
import ShopingSection3 from "../components/CartShoping/ShopingSection3.vue";
export default {
  name: "CartShoping",
  components: { ShopingSection1, ShopingSection2, ShopingSection3 },
};
</script>
