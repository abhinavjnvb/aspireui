<template>
  <div class="head-section">
    <div class="balance">
      <div class="balance-title open-sans-regular-14">Available balance</div>
      <div class="balance-value">
        <span class="currency open-sans-bold-13">$</span>
        <span class="open-sans-bold-26">3000</span>
      </div>
    </div>
    <div class="add-new-card">
      <button type="button" class="add-button open-sans-bold-13">
        <img src="../images/box.svg" alt="" />New Card
      </button>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.head-section {
  display: flex;
  justify-content: space-between;
  width: 100%;
}
.balance-title {
  color: #222222;
  padding: 0.5rem 0;
}
.currency {
  width: 20px;
  height: 18px;
  background-color: #01d167;
  color: #ffff;
  text-align: center;
  margin-right: 0.5rem;
}
.balance-value {
  display: flex;
  align-items: center;
}
.add-button {
  width: 110px;
  height: 30px;
  border: none;
  background: #325baf;
  border-radius: 4px;
  color: #fff;
  position: relative;
  padding-left: 0.5rem;
  margin-top: 1.5rem;
}
.add-button > img {
  position: absolute;
  left: 5px;
  top: 8px;
}
</style>
