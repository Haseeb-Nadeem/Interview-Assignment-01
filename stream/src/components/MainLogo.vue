<script setup>
import mainLogo from '@/assets/images/main-logo.png'
</script>

<template>
  <div class="text-center main-logo-theme mt-4">
    <router-link to="/" class="element-btn w-100 mb-4">
      <img :src="mainLogo" alt="main Logo" class="img-fluid" />
    </router-link>
  </div>
</template>
