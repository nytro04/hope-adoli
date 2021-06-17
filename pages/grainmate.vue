<template>
  <div class="my-40 overflow-hidden grain-mate">
    <div class="container mx-auto lg:justify-between lg:flex sm:px-10">
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
      <div class="mt-20 grain grain-bg-1"></div>
    </div>

    <div class="container mx-auto sm:px-10">
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
          they came up with a moisture meter for farmers to use, called
          GrainMate Moisture Meter.
        </p>
        <p class="text-gray-400 ">
          After about 2 years of exposing these local farmers to the GrainMate
          Moisture Moisture Moisture Meter and after receiving several feedbacks
          from them, there became a need to have a companion mobile app. The
          team reached out to me to design the mobile app.
        </p>
      </div>

      <div class="mt-10 lg:flex lg:justify-end">
        <img
          class="lg:w-4/6 lg:h-3/4"
          src="~/assets/img/farmer-img.png"
          alt=""
        />
      </div>

      <div class="mt-40 lg:flex lg:justify-between">
        <h3 class="mb-6 text-4xl font-bold lg:w-5/12">
          A beautiful design that solves problems.
        </h3>
        <p class="text-gray-400 lg:w-6/12">
          From our UX research of the 4 main target users, it became evident
          that the farmers were going to need the most help navigating the app.
          app. order to help them do so easily, I used colours on the
          backgrounds of of each tool to serve as a differentiator. Each tool
          was represented by a title, description and an illustration. Also, the
          tool that will used by them was placed in front.
        </p>
      </div>

      <div class="mt-20 md:flex md:items-center md:justify-between">
        <div class="md:w-5/12 ">
          <img src="~/assets/img/new/grainmate/img-01.png" alt="" />
        </div>
        <div class="mt-10 lg:mt-40 md:w-5/12">
          <img src="~/assets/img/new/grainmate/img-02.png" alt="" />
        </div>
      </div>
      <div class="mt-10 md:flex md:items-center md:justify-between">
        <div class="mb-10 md:w-5/12">
          <img src="~/assets/img/new/grainmate/img-03.png" alt="" />
        </div>
        <div class="lg:mt-40 md:w-5/12">
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
          users with very varying levels of understanding when it comes to the
          use of technology.
        </p>
      </div>
    </div>

    <div class="mb-40 ">
      <div class="mt-20 grain grain-bg-2 sm:px-0"></div>
    </div>

    <div class="container mx-auto sm:px-10">
      <div class="mt-20 md:flex md:items-center md:justify-between">
        <div class="md:w-5/12 ">
          <img src="~/assets/img/new/grainmate/img-05.png" alt="" />
        </div>
        <div class="mt-10 lg:mt-40 md:w-5/12">
          <img src="~/assets/img/new/grainmate/img-06.png" alt="" />
        </div>
      </div>
      <div class="mt-10 md:flex md:items-center md:justify-between">
        <div class="mb-10 md:w-5/12">
          <img src="~/assets/img/new/grainmate/img-07.png" alt="" />
        </div>
        <div class="lg:mt-40 md:w-5/12">
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
  </div>
</template>

<script>
export default {
  layout: 'pages',
  head() {
    return {
      title: 'Grainmate - Hope Adoli'
    }
  }
}
</script>

<style lang="scss" scoped>
@import './assets/scss/abstracts/_mixins.scss';

.grain-mate {
  @include respond(phone) {
    padding: 0 1rem;
  }
}

.grain {
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

  &-bg-1 {
    background-image: url('~/assets/img/new/grainmate/thumbnail.png');
  }
  &-bg-2 {
    background-image: url('~/assets/img/new/grainmate/video-thumbnail.png');
  }
}

/* .grain-bg-2 {
  height: 100vh;
  width: 100%;
  background-size: cover;
  background-position: center;
  background-color: #66aa8c;

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
} */
</style>
