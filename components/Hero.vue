<template>
  <div class="hero hero-lg bg-primary px-2">
    <div class="hero-body text-center px-2 mx-2">
      <img
        src="my-pic-no-bg.webp"
        class="me"
        alt="Abdulhakeem Adetunji Mustapha"
      />
      <h1 class="text-bold front">Abdulhakeem Adetunji Mustapha</h1>
      <p class="my-about front mb-2 pb-2" v-if="show === 1">
        I am a result-oriented Software Engineer with almost a decade of
        industry experience building amazing web applications, coordinating
        cross-functional teams, optimizing code for performance and simplifying
        complex technical details for non-technical stakeholders.
      </p>
      <p class="my-about front mb-2 pb-2" v-else>
        I'm a frontend developer who is not scared of the backend. With almost a
        decade experience in building and deploying mobile and web applications,
        I've become a real jack of all trade, master of pun. Not to brag, I
        consider myself to be among the top 1% of the best 1%.
      </p>
      <p class="text-warning text-large text-bold my-about">
        I'm looking for remote opportunities to join a diverse team building an
        awesome product. I'm open to fulltime, contract or freelance engagement.
      </p>
      <a
        href="https://docs.google.com/document/d/1xElMvl-O5xN6oA5U989hwJlEwEseLTA-QxpNFkxs73Q/edit?usp=sharing"
        target="_blank"
        rel="noreferrer"
        class="btn mt-2 text-uppercase text-bold bg-dark btn-primary"
        >Checkout my resume</a
      >

      <a
        href="mailto:abdulhakeemmustapha@gmail.com?subject=I've a Project for you&body=Hi Abdul,"
        class="btn mt-2 text-bold mx-2 text-uppercase"
        target="_blank"
        rel="noopener"
      >
        Hire Me
      </a>
      <div class="lnks">
        <a href="https://blog.amustapha.com" class="text-light" rel="noopener"
          >My Blog</a
        >
        <a
          href="mailto:abdulhakeemmustapha@gmail.com"
          class="text-light hide-md"
          rel="noopener"
        >
          abdulhakeemmustapha@gmail.com
        </a>
        <a href="tel:+2347067577058" class="text-light">+234 706 757 7058</a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Hero",
  computed: {
    show: function () {
      return Math.ceil(Math.random() * 2);
    },
  },
};
</script>

<style scoped>
.my-about {
  max-width: 680px;
  margin: auto;
}

.me {
  position: absolute;
  bottom: 0;
  left: 0;
  z-index: 1;
}

.lnks {
  position: absolute;
  top: 0;
  right: 0;
  padding: 24px;
}

.lnks a {
  padding: 16px;
}

.front {
  z-index: 20;
}

.hero {
  position: relative;
}

@media (min-width: 1146px) {
  .hero-body {
    margin-left: 256px !important;
  }
}

@media (min-width: 800px) {
  .hero-body {
    margin-left: 400px !important;
  }
}

@media (max-width: 800px) {
  .hero-body img {
    display: none;
  }
}
</style>
