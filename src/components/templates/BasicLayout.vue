<template>
  <div class="basic-layout d-flex flex-column h-100">
    <div class="d-flex flex-row h-100">
      <ActivityBar />

      <SideBar />

      <div class="content flex-fill">
        <router-view />
      </div>
    </div>

    <StatusBar />
  </div>
</template>

<script>
import ActivityBar from "@/components/organisms/ActivityBar.vue";
import SideBar from "@/components/organisms/SideBar.vue";
import StatusBar from "@/components/organisms/StatusBar.vue";

export default {
  name: "basic-layout",
  components: {
    ActivityBar,
    SideBar,
    StatusBar
  }
};
</script>

<style lang="scss">
.content {
  background-color: rgb(30, 30, 30);
}
</style>
