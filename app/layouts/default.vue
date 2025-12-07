<script setup lang="ts">
</script>

<template>
  <div>
    <UContainer class="sm:border-x border-default pt-4">
      <div class="border-b border-default">
        <AppHeader :links="navLinks" />
      </div>
      <slot />
      <AppFooter />
    </UContainer>
  </div>
</template>
