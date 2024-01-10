<template>
  <div>

    <!-- วนลูปผ่านรายการหมวดหมู่ -->
    <div v-for="category in categories" :key="category">
      <h3 class="text-center">{{ category }}</h3>
      <ProductList :category="category" />
    </div>
  </div>
</template>

<script setup>
import ProductList from "@/components/FrontEnd/ProductList.vue";

const categories = ["หูฟัง ", "หูฟัง Eadbud", "หูฟัง Full Size", "หูฟัง Gaming", "ลำโพงพกพา"];


</script>

<style>
</style>
