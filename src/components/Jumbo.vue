<template>
  <!-- JUMBOTRON PICTURES / BUTTONS / TITLES -->
  <div class="bg-jumbotron">
    <div
      class="container d-flex align-items-center flex-wrap g-3 py-3"
      id="jumbotron"
    >
      <div class="row">
        <div class="photo col-4">
          <button class="btn btn-blue">PHOTOGRAPHY</button>
          <h5>How To Take Better Pictures in 30 Seconds</h5>
        </div>
        <div class="gadgets col-4">
          <button class="btn btn-blue">GADGETS</button>
          <h5>Gadgets That Make Your Smartphone Even Smarter</h5>
        </div>
        <div class="travel col-4">
          <button class="btn btn-blue">TRAVEL</button>
          <h5>20 Top-Rated Tourist Attractions in Manhattan</h5>
        </div>
        <div class="life col-4">
          <button class="btn btn-blue">LIFESTYLE</button>
          <h5>The Best Way to Ride a Motorcycle</h5>
        </div>
        <div class="trip col-4">
          <button class="btn btn-blue">TRAVEL</button>
          <h5>5 Fun Things to Do at the Beach</h5>
        </div>
        <div class="recipes col-4">
          <button class="btn btn-blue">RECIPES</button>
          <h5>Amazingly Fresh Fruit And Herb Drinks For Summer</h5>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Jumbo",
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/style.scss";
</style>