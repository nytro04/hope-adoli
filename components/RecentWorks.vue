<template>
  <div class="recent-works">
    <h2 class="text-6xl font-semibold text-right">
      Recent works
    </h2>
    <span class="block mt-10 mb-32 border-t-2 border-white"></span>

    <div class="card-container">
      <div class="card-member member-1">
        <img src="~/assets/img/hope.png" alt="" />
        <h3 class="text-3xl font-semibold">
          GrainMate mobile
        </h3>
        <p>
          GrainMate app is supercharging African farmers and agribusinesses with
          the tools and resources they need to get to the next level ⚡️
        </p>
      </div>
      <div class="card-member member-2">
        <img src="~/assets/img/hope.png" alt="" />
        <h3 class="text-3xl font-semibold">
          GrainMate mobile
        </h3>
        <p>
          GrainMate app is supercharging African farmers and agribusinesses with
          the tools and resources they need to get to the next level ⚡️
        </p>
      </div>
      <div class="card-member member-1"></div>
    </div>
    <p>cool</p>
    <p>cool</p>
    <p>cool</p>
    <p>cool</p>
    <p>cool</p>
    <p>cool</p>
    <p>cool</p>
    <p>cool</p>
    <p>cool</p>
    <p>cool</p>
    <p>cool</p>
  </div>
</template>

<script>
export default {}
</script>

<style scoped>
.card-container {
  /* background: #000; */
  /* height: 80vh; */
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 15rem;
  /* grid-template-rows: auto 1fr 1fr 2fr 1fr 1fr; */
  grid-template-rows: repeat(6, 1fr);
}

/* .card-member {
  text-align: center;
} */

.member-1 {
  grid-row-start: 1;
  grid-column-start: 1;
  grid-row-end: 5;
}
.member-2 {
  grid-row-start: 2;
  grid-column-start: 2;
  grid-row-end: 5;
}
</style>
