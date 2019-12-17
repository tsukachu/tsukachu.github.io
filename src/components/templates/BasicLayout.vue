<template>
  <div class="basic-layout min-vh-100 d-flex flex-column">
    <div class="flex-fill d-flex flex-row">
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

  position: absolute;
  top: 0;
  bottom: 22px;
  left: 218px;
  right: 0;

  overflow-y: auto;
}
</style>
