<template>
  <div>
    <h1>Index</h1>
    <NuxtLink to="/login">Login</NuxtLink>
    <br><br>
    <button @click="testNavigate">Test Bug</button>
  </div>
</template>
<script lang="ts" setup>
const ROUTE_NAMES = {
  LOGIN: 'login',
};
const testNavigate = () => {
  navigateTo({ name: ROUTE_NAMES.LOGIN }, { open: { target: '_blank' } });
};
</script>
