<script setup lang="ts">
const color = useColorMode()
function toggleDark () {
  color.preference = color.value === 'dark' ? 'light' : 'dark'
}
</script>

<template>
  <button
    text-center
    class="!outline-none"
    @click="toggleDark"
  >
    <div
      inline-block
      dark:i-carbon-moon
      i-carbon-sun
    />
  </button>
</template>
