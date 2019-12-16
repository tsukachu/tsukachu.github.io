<template>
  <div class="activity-bar d-flex flex-column">
    <VerticalList :links="linksTop" />

    <VerticalList class="mt-auto" :links="linksBottom" />
  </div>
</template>

<script>
import VerticalList from "@/components/molecules/VerticalList.vue";

export default {
  name: "activity-bar",
  components: {
    VerticalList
  },
  data: function() {
    return {
      linksTop: [
        {
          to: "/",
          faPrefix: "fas",
          faName: "home"
        }
      ],
      linksBottom: [
        {
          to: "https://github.com/tsukachu/tsukachu.github.io",
          faPrefix: "fab",
          faName: "github",
          isExternal: true
        }
      ]
    };
  }
};
</script>

<style lang="scss">
.activity-bar {
  background-color: rgb(51, 51, 51);
  width: 48px;
}
</style>
