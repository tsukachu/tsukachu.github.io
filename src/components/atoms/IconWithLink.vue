<template>
  <div class="icon-with-link d-flex align-items-center justify-content-center">
    <a v-if="isExternal" :href="to" target="_blank">
      <font-awesome-icon :icon="[faPrefix, faName]" />
    </a>

    <router-link v-else :to="to">
      <font-awesome-icon :icon="[faPrefix, faName]" />
    </router-link>
  </div>
</template>

<script>
export default {
  name: "icon-with-link",
  props: {
    to: String,
    faPrefix: String,
    faName: String,
    isExternal: {
      type: Boolean,
      default: false
    }
  }
};
</script>

<style lang="scss">
.icon-with-link {
  height: 48px;
  width: 48px;

  margin-bottom: 4px;

  a {
    svg {
      font-size: 24px;
      color: rgba(255, 255, 255, 0.4);

      &:hover {
        color: rgb(255, 255, 255);
      }
    }
  }
}
</style>
