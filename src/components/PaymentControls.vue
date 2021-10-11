<template>
  <div v-for="control in controls" :key="control.id" class="group">
    <img :src="getImgUrl(control.src)" :alt="control.label" />
    <div class="control-name">{{ control.label }}</div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      controls: [
        { id: 1, label: "Freeze Card", src: "Freeze.svg" },
        { id: 2, label: "Set spend limit", src: "Limit.svg" },
        { id: 3, label: "Add to GPay", src: "GPay.svg" },
        { id: 4, label: "Replace card", src: "ReplaceCard.svg" },
        { id: 5, label: "CancelCard", src: "DeactivateCard.svg" },
      ],
    };
  },
  methods: {
    getImgUrl(pic) {
      return require("../images/" + pic);
    },
  },
};
</script>

<style scoped>
.group {
  padding: 0.5rem;
}

.control-name {
  /* width: 36px; */
}
</style>
