<script setup>
import {computed} from 'vue'
import MonitorPlayIcon from './MonitorPlayIcon.vue'

const props = defineProps({
  demoVideo: String,
})
</script>

<template>
  <a :href="demoVideo"
    target="_blank"
    v-if="demoVideo"
    class="text-sm inline-flex items-center rounded !no-underline px-2 py-1 leading-none border dark:border-white border-gray-900 hover:bg-gray-900 !text-gray-900 dark:!text-white hover:!text-white dark:hover:bg-white dark:hover:!text-gray-900"
  >
    <MonitorPlayIcon class="h-4 inline mr-1 dark:stroke-white" /> Watch the demo video
  </a>
</template>
