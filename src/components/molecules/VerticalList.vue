<template>
  <ul class="nav flex-column">
    <li v-for="link in links" :key="link.id">
      <IconWithLink v-bind="link" />
    </li>
  </ul>
</template>

<script>
import IconWithLink from "@/components/atoms/IconWithLink.vue";

export default {
  name: "vertical-list",
  components: {
    IconWithLink
  },
  props: {
    links: Array
  }
};
</script>
