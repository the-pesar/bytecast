<template>
  <div>{{ `ByteCast is building${dots}` }}</div>
</template>
<script lang="ts" setup>
const dots = ref<string>("")

setInterval(() => {
  if (dots.value.length < 6) dots.value += "."
  else dots.value = ""
}, 500)
</script>
<style>
div {
  font-family: monospace;
  font-size: 24px;
}
</style>
