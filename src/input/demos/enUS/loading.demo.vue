<markdown>
# Loading

`input` has a loading state.

Note: When using `clearable`, `suffix` and `loading` at the same time, and `loading` is `false`, there will be a space between the clear button and the suffix, if you want to remove the whitespace, `loading` should be set to `undefined` when stopping loading.
</markdown>

<script lang="ts" setup>
import { ref } from 'vue'

const value = ref(null)
</script>

<template>
  <n-input
    v-model:value="value"
    type="text"
    placeholder="Basic Input"
    loading
  />
</template>
