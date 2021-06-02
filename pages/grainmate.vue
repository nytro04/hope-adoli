<template>
  <div class="my-40 overflow-hidden grain-mate">
    <div class="lg:justify-between lg:flex">
      <div class="lg:w-6/12">
        <h1 class="heading heading__primary">
          GrainMate <br />
          mobile app
        </h1>
        <p class="mt-8 mb-10 text-gray-400">
          Sesi technologies • 2020
        </p>
      </div>

      <div class=" lg:w-6/12">
        <h3 class="mb-6 text-4xl font-bold text-gray-400 ">
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
          <a
            class="font-bold"
            href="https://play.google.com/store/apps/details?id=com.sesitechnologies.grainmateapp&hl=en&gl=US"
            target="_blank"
            rel="noopener noreferrer"
          >
            Download on Google Playstore
          </a>
        </div>
      </div>
    </div>

    <div class="mb-40 full-width">
      <div class="mt-20 grain-bg"></div>
    </div>

    <div class="lg:w-5/12">
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

    <div class="mt-10 lg:flex lg:justify-end">
      <img class="lg:w-4/6 lg:h-3/4" src="~/assets/img/farmer-img.png" alt="" />
    </div>

    <div class="mt-40 lg:flex lg:justify-between">
      <h3 class="mb-6 text-4xl font-bold lg:w-5/12">
        A beautiful design that solves problems.
      </h3>
      <p class="text-gray-400 lg:w-6/12">
        From our UX research of the 4 main target users, it became evident that
        the farmers were going to need the most help navigating the app. In
        order to help them do so easily, I used colours on the backgrounds of
        each tool to serve as a differentiator. Each tool was represented by a
        title, description and an illustration. Also, the tool that will used by
        them was placed in front.
      </p>
    </div>

    <div class="mt-20 lg:flex lg:items-center lg:justify-between">
      <div class="lg:w-5/12 ">
        <img src="~/assets/img/new/grainmate/img-01.png" alt="" />
      </div>
      <div class="mt-10 lg:mt-40 lg:w-5/12">
        <img src="~/assets/img/new/grainmate/img-02.png" alt="" />
      </div>
    </div>
    <div class="mt-10 lg:flex lg:items-center lg:justify-between">
      <div class="mb-10 lg:w-5/12">
        <img src="~/assets/img/new/grainmate/img-03.png" alt="" />
      </div>
      <div class="lg:mt-40 lg:w-5/12">
        <img src="~/assets/img/new/grainmate/img-04.png" alt="" />
      </div>
    </div>

    <div class="mt-40 lg:flex lg:justify-between">
      <h3 class="mb-6 text-4xl font-bold lg:w-5/12">
        Designing for 10,000+ unique set of target user base.
      </h3>
      <p class="text-gray-400 lg:w-6/12">
        One of the most exciting things about this project was unlearning most
        things I knew about farming and agriculture as a whole, and then
        learning new behaviours from farmers, warehouse managers,
        agribusinesses, agri enthusiasts and learners among others. The
        uniqueness of this project lies in the target user base: a group of
        users with very varying levels of understanding when it comes to the use
        of technology.
      </p>
    </div>

    <div class="mb-40 full-width">
      <div class="mt-20 grain-bg-2"></div>
    </div>

    <div class="mt-20 lg:flex lg:items-center lg:justify-between">
      <div class="lg:w-5/12 ">
        <img src="~/assets/img/new/grainmate/img-05.png" alt="" />
      </div>
      <div class="mt-10 lg:mt-40 lg:w-5/12">
        <img src="~/assets/img/new/grainmate/img-06.png" alt="" />
      </div>
    </div>
    <div class="mt-10 lg:flex lg:items-center lg:justify-between">
      <div class="mb-10 lg:w-5/12">
        <img src="~/assets/img/new/grainmate/img-07.png" alt="" />
      </div>
      <div class="lg:mt-40 lg:w-5/12">
        <img src="~/assets/img/new/grainmate/img-08.png" alt="" />
      </div>
    </div>

    <span class="block mt-10 mb-32 border-t-2 border-white"></span>
    <h3 class="mb-10 text-2xl lg:text-6xl md:text-4xl">
      Get In touch
    </h3>

    <h2 class="my-10 text-2xl lg:text-6xl md:text-4xl">
      Other projects: Wacomm, Adiutor, Homechow, Farm For Me, MicroBis
    </h2>
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
@import './assets/scss/abstracts/_mixins.scss';

.grain-mate {
  @include respond(phone) {
    padding: 0 1rem;
  }
}

.grain-bg {
  background-image: url('~/assets/img/new/grainmate/thumbnail.png');
  height: 100vh;
  width: 100%;
  background-size: cover;
  background-position: center;
  background-color: #11905c;

  @include respond(tab-land) {
    height: 60vh;
  }
  @include respond(tab-port) {
    height: 50vh;
  }

  @include respond(phone) {
    height: 30vh;
    width: 100%;
  }
}

.grain-bg-2 {
  background-image: url('~/assets/img/new/grainmate/video-thumbnail.png');
  height: 100vh;
  width: 100%;
  background-size: cover;
  background-position: center;
  background-color: #66aa8c;

  @include respond(tab-land) {
    height: 50vh;
  }
  @include respond(tab-port) {
    height: 30vh;
  }
  @include respond(phone) {
    height: 30vh;
    width: 100%;
  }
}

.full-width {
  margin-left: -7rem;
  margin-right: -7rem;
}

.card-container {
  height: 80vh;
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  column-gap: 15rem;
  /* grid-template-rows: auto 1fr 1fr 2fr 1fr 1fr; */
  grid-template-rows: repeat(6, 1fr);

  @include respond(tab-land) {
    column-gap: 8rem;
    height: 90vh;
    margin-bottom: 0;
  }

  @include respond(tab-port) {
    column-gap: 8rem;
    height: 70vh;
    margin-bottom: 0;
  }

  @include respond(phone) {
    display: block;
    /* height: 150vh; */
    height: auto;
  }
}

.member-1 {
  grid-row-start: 1;
  grid-column-start: 1;
  grid-row-end: 5;

  /* @include respond(tab-land) {
    height: 50vh;
  }
  @include respond(tab-port) {
    height: 30vh;
  }
  @include respond(phone) {
    height: 30vh;
  } */
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
