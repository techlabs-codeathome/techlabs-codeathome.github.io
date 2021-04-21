<template>
  <ul class="flex items-center space-x-4">
    <li>
      <a href="https://techlabs-community.slack.com" class="hover:text-pink-600"
        ><TIcon icon="slack" :class="isSmall ? 'text-xl' : 'text-4xl'"
      /></a>
    </li>
    <li>
      <a
        href="https://www.techlabs.org/program/remote"
        class="hover:text-pink-600"
        ><TIcon icon="link" :class="isSmall ? 'text-xl' : 'text-4xl'"
      /></a>
    </li>
    <li>
      <a href="https://www.instagram.com/techlabs" class="hover:text-pink-600"
        ><TIcon icon="instagram" :class="isSmall ? 'text-xl' : 'text-4xl'"
      /></a>
    </li>
    <li v-if="showTechlabsLink">
      <a
        href="#"
        class="flex items-center px-4 py-2 space-x-2 border-2 border-gray-700 rounded-xl hover:border-pink-600 hover:text-pink-600"
        ><span><TIcon icon="link" class="text-xl" /></span
        ><span>techlabs.org</span></a
      >
    </li>
  </ul>
</template>

<script>
import { defineComponent } from '@nuxtjs/composition-api'
export default defineComponent({
  props: {
    isSmall: {
      type: Boolean,
    },
    showTechlabsLink: {
      type: Boolean,
    },
  },
  setup() {
    return {}
  },
})
</script>
