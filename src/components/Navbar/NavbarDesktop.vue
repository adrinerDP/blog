<template>
  <nav class="hidden md:block lg:block xl:block items-center justify-between flex-wrap container mx-auto py-1 z-20 dark:text-gray-400">
    <div class="flex-grow flex items-center w-auto mx-4">
      <div class="flex items-center flex-shrink-0 mr-4">
        <span class="font-semibold text-lg tracking-tight">{{ $static.metadata.siteName }}</span>
      </div>
      <div class="flex-grow">
        <ul class="list-none flex justify-left">
          <li v-for="navItem in $static.metadata.headerNavigation" :key="navItem.name" class="px-4 py-1">
            <g-link class="block py-1" :to="navItem.link" :title="navItem.name" v-if="!navItem.external">
              <font-awesome :icon="navItem.icon" :fixedWidth="true" v-if="navItem.icon" />
              {{ navItem.name }}
            </g-link>
            <a class="block" :href="navItem.link" target="_blank" :title="navItem.name" v-if="navItem.external">
              <font-awesome :icon="navItem.icon" :fixedWidth="true" v-if="navItem.icon" />
              {{ navItem.name }}
            </a>
          </li>
        </ul>
      </div>

      <div class="inline-block">
        <ul class="list-none flex justify-center md:justify-end">
          <li class="mr-6">
            <search-button v-on="$listeners"></search-button>
          </li>
          <li>
            <theme-switcher v-on="$listeners" :theme="theme"/>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<script>
import ThemeSwitcher from "~/components/Navbar/ThemeSwitcher.vue";
import SearchButton from "~/components/Navbar/SearchButton.vue";

export default {
  data: function() {
    return {
      vcoConfig: {
        events: ["dblclick", "click"],
        isActive: true
      }
    };
  },
  components: {
    ThemeSwitcher,
    SearchButton
  },
  props: {
    theme: {
      type: String
    }
  },
};
</script>

<static-query>
query {
  metadata {
    siteName
    headerNavigation {
      name
      link
      external
      icon
    }
  }
}
</static-query>
