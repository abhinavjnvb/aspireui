<template>
  <div class="order-group">
    <div class="group-1 flex-row">
      <div class="circle">
        <img :src="getImgUrl(image)" alt="" />
      </div>
      <div class="order_name">
        <p class="open-sans-semi-bold-14">Hamleys</p>
        <span class="open-sans-regular-14">20 May 2020</span>
        <div class="order_detail">
          <img src="../images/file-storage.svg" />
          <span class="open-sans-regular-14 ">Charged to debit card</span>
        </div>
      </div>
    </div>
    <div class="price open-sans-semi-bold-14">+ S$ 150</div>
  </div>
</template>

<script>
export default {
  props: ["image"],
  methods: {
    getImgUrl(pic) {
      return require("../images/" + pic);
    },
  },
};
</script>

<style scoped>
.order-group {
  margin: 1rem 0;
  display: flex;
  justify-content: space-between;
  padding: 0 12px;
}
.circle {
  background: #009dff1a;
  width: 48px;
  height: 48px;
  border-radius: 50%;
  position: relative;
  margin-right: 0.5rem;
}
.circle > img {
  position: absolute;
  top: 16px;
  left: 16px;
}
.order_name > p {
  color: #222222;
}
.order_name > span {
  color: #aaaaaa;
  margin-bottom: 10px;
}
.order_detail > span {
  color: #325baf;
  margin-top: 6px;
}
.order_detail > img {
  padding-right: 6px;
}
.price {
  color: #01d167;
}
</style>
