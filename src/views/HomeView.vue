<template>
  <div class="home container">
    <HomeSection1 />
    <HomeSection2 />
    <HomeSection3 />
  </div>
</template>

<script>
import HomeSection1 from "../components/Home/HomeSection1.vue";
import HomeSection2 from "@/components/Home/HomeSection2.vue";
import HomeSection3 from "@/components/Home/HomeSection3.vue";
// @ is an alias to /src

export default {
  name: "HomeView",
  components: { HomeSection1, HomeSection2, HomeSection3 },
};
</script>
