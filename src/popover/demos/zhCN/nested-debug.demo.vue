<markdown>
# Nested Debug
</markdown>

<script lang="ts" setup>
const dataList = [
  'Lorem',
  'Lorem',
  'Lorem ipsum, dolor sit amet consectetur adipisicing elit. Vero eveniet exercitationem quasi. Sequi quia natus quam ipsa sit autem eveniet harum tempore, eius placeat temporibus nobis veritatis vero totam possimus.',
  'jflakjdflksjflkajdlkfjaslkfjklasjdflkasjflkjsadlkf'
]
</script>

<template>
  <n-popover trigger="click" placement="bottom-end">
    <template #trigger>
      <div>
        <n-tag>hover</n-tag>
      </div>
    </template>
    <n-list bordered>
      <n-list-item v-for="(item, index) in dataList" :key="index">
        <n-ellipsis style="max-width: 300px">
          {{ item }}
        </n-ellipsis>
      </n-list-item>
    </n-list>
  </n-popover>
</template>
