<template>
  <div>
    <div class="w-full mb-2 overflow-x-hidden dark:text-gray-400">
      <h2 class="text-xl font-semibold m-0">
        {{ $static.metadata.siteName }}
      </h2>
      <hr class="my-6 w-8 border-black">
      <div class="menu-links">
        <ul>
          <li v-for="navItem in $static.metadata.headerNavigation" :key="navItem.name" class="py-1">
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
    </div>
  </div>
</template>

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
