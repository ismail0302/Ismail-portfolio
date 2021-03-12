<template>
  <nav class="flex items-center justify-between flex-wrap bg-indigo-600 p-2 bottom-0 z-10">
    <div class="flex-grow flex items-center w-auto">
      <div class="text-sm flex-grow">
        <NuxtLink
          to="/legal/"
          no-prefetch
          rel="nofollow"
          class="inline-block mt-0 mr-2 text-white hover:text-indigo-100 no-underline"
          v-text="'Legal notice'"
        />
        <NuxtLink
          to="/privacy/"
          no-prefetch
          rel="nofollow"
          class="inline-block mt-0 text-white hover:text-indigo-100 no-underline"
          v-text="'Privacy Policy'"
        />
      </div>
    </div>
  </nav>
</template>
<script>
import { version } from '~/package.json'

export default {
  components: {
  },
  version
}
</script>
