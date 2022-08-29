<template>
  <div>
    <TestComponent></TestComponent>
    <pre>{{ c }}</pre>
  </div>
</template>

<script setup lang="ts">
  const a = ref(true)
  const b = ref(false)

  const c = computed(() => a.value && b.value)
</script>
