<script setup lang="ts">
import type { NavigationMenuItem } from '@nuxt/ui'

defineProps<{
  links: NavigationMenuItem[]
}>()
</script>

<template>
  <UNavigationMenu
    :items="links"
    variant="link"
    color="neutral"
    class="backdrop-blur-sm"
    :ui="{
      link: 'px-2 py-1',
      linkLeadingIcon: 'hidden'
    }"
  >
    <template #list-trailing>
      <ColorModeButton />
    </template>
  </UNavigationMenu>
</template>
