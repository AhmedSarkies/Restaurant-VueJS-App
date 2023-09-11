<script>
import {
  HeaderVue,
  LandingHeroVue,
  CategoriesVue,
  SpecialDishes,
  TestimonialsVue,
  ServicesVue,
  FooterVue,
} from "@/components";

export default {
  components: {
    HeaderVue,
    LandingHeroVue,
    CategoriesVue,
    SpecialDishes,
    TestimonialsVue,
    ServicesVue,
    FooterVue,
  },
  name: "HomeView",
};
</script>

<template>
  <div>
    <header-vue />
    <landing-hero-vue />
    <categories-vue />
    <special-dishes />
    <testimonials-vue />
    <services-vue />
    <footer-vue />
  </div>
</template>

<style lang="scss" scoped></style>
