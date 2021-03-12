<template>
  <nav class="flex items-center justify-between flex-wrap bg-red-600 p-4 sticky top-0 z-10">
    <NuxtLink to="/" class="flex items-center flex-no-shrink text-white mr-6 no-underline">
      <span class="font-semibold text-xl tracking-tight">
        Home
      </span>
    </NuxtLink>
    <div
      class="block lg:hidden"
    >
      <button
        class="flex items-center px-3 border rounded text-red-300 border-red-400 w-10 hover:text-white hover:border-white"
        @click="toggleVisibility"
      >
        <Icon
          view-box="0 0 20 20"
          icon-title="Menu"
          path="M0 3h20v2H0V3zm0 6h20v2H0V9zm0 6h20v2H0v-2z"
        />
      </button>
    </div>
    <div
      :class="{'hidden': !isVisible}"
      class="w-full lg:block flex-grow lg:flex lg:items-center lg:w-auto"
    >
      <div class="text-sm lg:flex-grow">
        <div
          v-for="item in navItems"
          :key="item.name"
          class="block mt-4 lg:inline-block lg:mt-0 mr-4"
        >
          <NuxtLink
            :to="item.link"
            class="text-red-200 hover:text-white no-underline"
            @click.native="toggleVisibility"
          >
            {{ item.name }}
          </NuxtLink>
        </div>
      </div>
      </div>
  </nav>
</template>
<script>
import { ref } from '@nuxtjs/composition-api'
import Icon from '~/components/Icon.js'

export default {
  components: {
    Icon
  },
  setup () {
    const isVisible = ref(false)
    const toggleVisibility = () => {
      isVisible.value = !isVisible.value
    }

    return {
      isVisible,
      navItems: [
        {
          name: 'Projects',
          link: '/timeline/'
        },
        {
          name: 'Support me',
          link: '/support-me/'
        }
      ],
      toggleVisibility
    }
  }
}
</script>
