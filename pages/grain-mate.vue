<template>
  <div class="my-40 grain-mate">
    <div class="flex justify-between">
      <div class="w-6/12">
        <h1 class="heading heading__primary">
          GrainMate <br />
          mobile app
        </h1>
        <p class="mt-8 text-gray-400">
          Sesi technologies • 2020
        </p>
      </div>

      <div class="w-6/12">
        <h3 class="mb-6 text-4xl font-bold text-gray-400">
          Overview
        </h3>
        <p class="text-gray-400">
          Meet GrainMate app: A companion of GrainMate moisture meter. While the
          moisture meter is used to measure the moisture content in grains, the
          app uses the result to suggest a solution. But that’s not all. The
          app’s Learn feature curates mini lessons on Post Harvest Loss (PHL)
          and how to prevent/manage it. It also has a marketplace for
          agribusinesses to sell agricultural products.
        </p>

        <div class="mt-8">
          <nuxt-link to="">
            Download on Google Playstore
          </nuxt-link>
        </div>
      </div>
    </div>

    <div class="mb-40 full-width">
      <div class="mt-20 grain-bg"></div>
    </div>

    <div class="w-5/12">
      <h3 class="mb-6 text-4xl font-bold text-gray-400">
        The challenge
      </h3>
      <p class="mb-5 text-gray-400">
        Sesi Technologies’ primary target is to use technology to help reduce
        the alarming occurrence of Post Harvest Loss (PHL) being witnessed by
        grain farmers across Africa, especially Ghana.
      </p>
      <p class="mb-5 text-gray-400">
        As of December 2019, it was estimated that
        <span class="font-semibold text-white">
          Ghana losses close to USD 141 million in cereals due to PHL😱.
        </span>
        So in order to achieve the goal of minimising the occurrence of same,
        they came up with a moisture meter for farmers to use, called GrainMate
        Moisture Meter.
      </p>
      <p class="text-gray-400 ">
        After about 2 years of exposing these local farmers to the GrainMate
        Moisture Moisture Moisture Meter and after receiving several feedbacks
        from them, there became a need to have a companion mobile app. The team
        reached out to me to design the mobile app.
      </p>
    </div>

    <div class="flex justify-end mt-10">
      <img class="w-4/6 h-3/4" src="~/assets/img/farmer-img.png" alt="" />
    </div>

    <div class="flex justify-between mt-40">
      <h3 class="w-5/12 mb-6 text-4xl font-bold">
        A beautiful design that solves problems.
      </h3>
      <p class="w-6/12">
        From our UX research of the 4 main target users, it became evident that
        the farmers were going to need the most help navigating the app. In
        order to help them do so easily, I used colours on the backgrounds of
        each tool to serve as a differentiator. Each tool was represented by a
        title, description and an illustration. Also, the tool that will used by
        them was placed in front.
      </p>
    </div>

    <div class="mt-32 card-container">
      <div class="card-member member-1">
        <div class="first-img jarallax">
          <img src="~/assets/img/img-01.png" alt="" class="jarallax-img" />
          <div class="para-img"></div>
        </div>
      </div>
      <div class="card-member member-2">
        <div class=" jarallax">
          <img
            src="~/assets/img/img-02.png"
            alt=""
            class="jarallax-img wa-bg"
          />
          <div class="para-img"></div>
        </div>
      </div>
    </div>

    <div class="mb-32 card-container">
      <div class="card-member member-1">
        <div class="first-img jarallax">
          <img src="~/assets/img/img-03.png" alt="" class="jarallax-img" />
          <div class="para-img"></div>
        </div>
      </div>
      <div class="card-member member-2">
        <div class=" jarallax">
          <img
            src="~/assets/img/img-04.png"
            alt=""
            class="jarallax-img wa-bg"
          />
          <div class="para-img"></div>
        </div>
      </div>
    </div>

    <div class="flex justify-between mt-40">
      <h3 class="w-5/12 mb-6 text-4xl font-bold">
        Designing for 10,000+ unique set of target user base.
      </h3>
      <p class="w-6/12">
        One of the most exciting things about this project was unlearning most
        things I knew about farming and agriculture as a whole, and then
        learning new behaviours from farmers, warehouse managers,
        agribusinesses, agri enthusiasts and learners among others. The
        uniqueness of this project lies in the target user base: a group of
        users with very varying levels of understanding when it comes to the use
        of technology.
      </p>
    </div>

    <div class="mb-40 full-width ">
      <div class="mt-20 grain-bg-2"></div>
    </div>

    <div class="mb-32 card-container">
      <div class="card-member member-1">
        <div class="first-img jarallax">
          <img src="~/assets/img/img-06.png" alt="" class="jarallax-img" />
          <div class="para-img"></div>
        </div>
      </div>
      <div class="card-member member-2">
        <div class=" jarallax">
          <img
            src="~/assets/img/img-07.png"
            alt=""
            class="jarallax-img wa-bg"
          />
          <div class="para-img"></div>
        </div>
      </div>
    </div>

    <div class="mb-32 card-container">
      <div class="card-member member-1">
        <div class="first-img jarallax">
          <img src="~/assets/img/img-08.png" alt="" class="jarallax-img" />
          <div class="para-img"></div>
        </div>
      </div>
      <div class="card-member member-2">
        <div class=" jarallax">
          <img
            src="~/assets/img/img-09.png"
            alt=""
            class="jarallax-img wa-bg"
          />
          <div class="para-img"></div>
        </div>
      </div>
    </div>

    <span class="block mt-10 mb-32 border-t-2 border-white"></span>
    <h3 class="mb-10 text-7xl">
      Get In touch
    </h3>

    <h2 class="w-4/5 my-10 text-7xl">
      Other projects: Wacomm, Adiutor, Homechow, Farm For Me, MicroBis
    </h2>
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.grain-bg {
  background-image: url('~/assets/img/hero-section-img.png');
  height: 90vh;
  width: 100%;
  background-size: cover;
  background-position: center;
  background-color: #11905c;
}
.grain-bg-2 {
  background-image: url('~/assets/img/img-05.png');
  height: 90vh;
  width: 100%;
  background-size: cover;
  background-position: center;
  background-color: #66aa8c;
}

.full-width {
  margin-left: -5rem;
  margin-right: -5rem;
}

.card-container {
  height: 80vh;
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  column-gap: 15rem;
  /* grid-template-rows: auto 1fr 1fr 2fr 1fr 1fr; */
  grid-template-rows: repeat(6, 1fr);

  .para-img {
    height: 35rem;
  }
}

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

.first-img {
  background-color: #11905c;
}
.third-img {
  background-color: #c9c9c9;
}
.fourth-img {
  background-color: #f6dacc;
}
</style>
