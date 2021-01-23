<template>
  <div>
    <div class="z-100 text-center bg-gray-200 dark:bg-gray-900 dark:text-gray-200 lg:py-14 md:py-10 py-8" v-if="!hasImage">
      <h1 v-if="title!=null" class="h3 mb-1 font-extrabold">{{ title }}</h1>
      <p v-if="sub!=null" class="h6 m-0 font-serif">{{ sub }}</p>
    </div>

    <div v-if="hasImage" class="z-100 relative mt-0 h-auto">
      <g-image v-if="hasImage && staticImage" :src="require(`!!assets-loader!@pageImage/${image}`)" width="1400" height="400" class="object-cover absolute -z-10 h-full w-full" />
      <g-image v-if="hasImage && !staticImage" :src="image" width="1400" height="400" class="object-cover absolute -z-10 h-full w-full" />
      <slot>
        <div class="text-center text-white bg-gray-800 lg:py-14 md:py-10 py-8" :class='`bg-opacity-${opacity}`'>
          <h1 v-if="title!=null" class="h3 mb-1 font-extrabold">{{ title }}</h1>
          <p v-if="sub!=null" class="h6 m-0 font-serif">{{ sub }}</p>
        </div>
      </slot>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    title: {
      type: String,
      default: null
    },
    sub: {
      type: String,
      default: null
    },
    image: {
      type: String | Object,
      default: null
    },
    staticImage: {
      type: Boolean,
      default: true
    },
    opacity: {
      type: Number,
      default: 50
    }
  },
  computed: {
    hasImage() {
      return !!this.image;
    }
  }
};
</script>

<style>
</style>
