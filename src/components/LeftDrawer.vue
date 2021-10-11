<template>
  <div class="left-drawer">
    <img src="../images/Logo.svg" alt="aspire" />
    <div class="description open-sans-regular-15">
      Trusted way of banking for 3,000+ <br />SMEs and startups in Singapore
    </div>
    <ul>
      <li v-for="tab in tabs" :key="tab.id">
        <span><img :src="getImgUrl(tab.src)" :alt="tab.label"/></span>
        <span
          :class="[
            'tab-name',
            'open-sans-regular-16',
            tab.id == 2 ? 'active' : '',
          ]"
          >{{ tab.label }}</span
        >
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      tabs: [
        { id: 1, label: "Home", src: "Home.svg" },
        { id: 2, label: "Cards", src: "Card.svg" },
        { id: 3, label: "Payments", src: "Payments.svg" },
        { id: 4, label: "Credit", src: "Credit.svg" },
        { id: 5, label: "Settings", src: "Account.svg" },
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
.left-drawer {
  flex: 0.25;
  padding-top: 3rem;
  background-color: #0c365a;
  padding-left: 40px;
}
.active {
  color: #01d167 !important;
}
.description {
  margin: 1.2rem 0 5rem 0;
  color: #ffffff;
  opacity: 30%;
}
ul {
  list-style: none;
}
li {
  display: flex;
  /* justify-content: center; */
  align-items: center;
  margin-bottom: 3rem;
}
.tab-name {
  padding: 0 1rem;
  color: #ffff;
  cursor: pointer;
}
</style>
