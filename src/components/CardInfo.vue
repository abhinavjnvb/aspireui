<template>
  <div class="card-info">
    <div class="show-details open-sans-bold-12">
      <img src="../images/eye.svg" /><span>Show card number</span>
    </div>
    <div class="card-details">
      <img src="../images/AspireLogo.svg" alt="logo" />
      <h3 class="card-holder-name open-sans-bold-24">Mark Henry</h3>
      <div class="card-number">
        **** **** **** ****
      </div>
      <div class="flex-row">
        <div class="validity open-sans-bold-13">
          <span>Thru: </span><span>12/20</span>
        </div>
        <div class="cvv open-sans-bold-13">
          <span>CVV: </span><span>***</span>
        </div>
      </div>

      <img class="visa" src="../images/VisaLogo.svg" alt="logo" />
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.card-info {
}

.show-details {
  color: #01d167;
  display: flex;
  justify-content: flex-end;
  padding: 0.4rem;
  color: #01d167;
  cursor: pointer;
}
.card-details {
  width: 410px;
  height: 250px;
  background-color: #01d167;
  border-radius: 8px;
  padding: 1rem;
}
.card-details > img {
  float: right;
  padding-top: 1rem;
  padding-right: 1rem;
}
.card-holder-name {
  padding-top: 3.5rem;
  padding-bottom: 2rem;
}
.card-number {
  font-size: 24px;
}
.visa {
}
.validity {
  margin-right: 36px;
}
</style>
