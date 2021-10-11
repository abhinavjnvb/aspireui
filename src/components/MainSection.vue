<template>
  <div class="container">
    <div class="wrapper">
      <head-section />
      <div class="payment-wrapper">
        <div class="tabs-options">
          <div class="tabs-1 open-sans-bold-14">My debit cards</div>
          <div class="tabs-2 open-sans-bold-14">All company cards</div>
        </div>
        <div class="payment-container">
          <div class="sub-container-1">
            <card-info />
            <div class="payment-controls open-sans-regular-13">
              <payment-controls />
            </div>
          </div>
          <div class="sub-container-2">
            <div class="card-details-section sec-1">
              <div class="flex-row">
                <img
                  src="../images/Details.svg"
                  alt="img"
                  class="details-icon"
                /><span class="open-sans-regular-14 ">Card Details</span>
              </div>
              <img src="../images/down-arrow.svg" alt="down" />
            </div>
            <div class="expanded">
              <div class="card-details-section ">
                <div class="flex-row">
                  <img
                    src="../images/transactions.svg"
                    alt="img"
                    class="details-icon"
                  /><span class="open-sans-regular-14 ">Card Details</span>
                </div>
                <img src="../images/up-arrow.svg" alt="up" />
              </div>
              <order-detail image="file-storage.svg"></order-detail>
              <hr />
              <order-detail image="flights.svg"></order-detail>
              <hr />
              <order-detail image="megaphone.svg"></order-detail>
              <hr />
              <order-detail image="file-storage.svg"></order-detail>
            </div>
            <div class="card-details-section sec-1 justify-center">
              <div class="view-transactions open-sans-semi-bold-13">
                View all card transactions
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import CardInfo from "./CardInfo.vue";
import HeadSection from "./HeadSection.vue";
import OrderDetail from "./OrderDetail.vue";
import PaymentControls from "./PaymentControls.vue";
export default {
  components: { HeadSection, CardInfo, PaymentControls, OrderDetail },
};
</script>

<style scoped>
.container {
  flex: 0.75;

  padding-top: 3rem;
  padding-left: 3rem;
  padding-right: 3rem;
}
hr {
  border: 1px solid #fcfcfc;
}
.wrapper {
  width: 100%;
}
.tabs-options {
  display: flex;
  padding: 1.5rem 0;
}
.tabs-1 {
  border-bottom: 1px solid #01d167;
}
.tabs-2 {
  color: #222222;
  opacity: 30%;
  margin-left: 32px;
}
.payment-container {
  color: #ffffff;
  border: 1px solid #fcfcfc;
  border-radius: 8px;
  /* height: 500px; */
  padding: 1.5rem;
  box-shadow: #00000014 0 2px 12px;
  display: flex;
}

.payment-controls {
  background-color: #edf3ff;
  border-radius: 1rem;
  padding: 1rem;
  margin-top: 2rem;
  display: flex;
  color: #0c365a;
}

.sub-container-1,
.sub-container-2 {
  flex: 0.5;
}
.card-details-section {
  background-color: #f5f9ff;
  border: 1px solid #f5f5f5;
  box-shadow: 1px solid #0000000a;
  color: #0c365a;
  display: flex;
  justify-content: space-between;
  padding: 1.5rem;
  border-radius: 8px;
}
.card-section-2 {
  background-color: #f5f9ff;
  border: 1px solid #f5f5f5;
  box-shadow: 1px solid #0000000a;
  color: #0c365a;
  display: flex;
  justify-content: space-between;
  padding: 1.5rem;
  border-radius: 8px;
  /* margin-top: 1.8rem;
    margin-left: 2rem; */
}
.sec-1 {
  margin-top: 1.8rem;
  margin-left: 2rem;
}

.expanded {
  margin-top: 1.8rem;
  margin-left: 2rem;
  border: 1px solid #f0f0f0;
  border-radius: 8px;
}
.view-transactions {
  color: #01d167;
  text-align: center;
}
</style>
