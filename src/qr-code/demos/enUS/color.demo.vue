<markdown>
  # Color

  Let the QR code no longer monotonous.
</markdown>

<script lang="ts" setup>
import { ref } from 'vue'

const color = ref('#225A95FF')
</script>

<template>
  <n-flex>
    <n-qr-code value="https://www.naiveui.com/" color="#18a058" />
    <n-qr-code
      value="https://www.naiveui.com/"
      color="#409eff"
      background-color="#F5F5F5"
    />
  </n-flex>
  <n-flex vertical>
    <n-color-picker v-model:value="color" />
    <n-qr-code
      value="https://www.naiveui.com/"
      :color="color"
      background-color="#F5F5F5"
    />
  </n-flex>
</template>
