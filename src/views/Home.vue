<script>
import Welcome from "../components/Home/Welcome.vue";
import Section1 from "../components/Home/Section1.vue";
import Section2 from "../components/Home/Section2.vue";
import Section3 from "../components/Home/Section3.vue";

import Section4 from "../components/Home/Section4.vue";
import Section5 from "../components/Home/Section5.vue";
import Foote from "../components/Home/Foote.vue";

export default {
  name: "App",
  components: {
    Welcome,
    Section1,
    Section2,
    Section3,
    Section4,
    Section5,
    Foote
  },
};
</script>



<template>
  <div class="home">
    <div class="home-container">
      <div class="section-0">
        <Welcome />
      </div>

      <div class="section-1">
        <Section1 />
      </div>

      <div class="section-0">
        <Section2 />
      </div>

      <div class="section-1">
        <Section3 />
      </div>

      <div class="section-0">
        <Section4 />
      </div>

      <div class="section-1">
        <Section5 />
      </div>

      <div class="section-0">
        <Foote />
      </div>
    </div>
  </div>
</template>



<style >
.home {
  display: flex;
  width: 100%;
  justify-content: center;
}

.home-container {
  display: block;
  width: 100%;
}

.section-0 {
  display: flex;
  justify-content: center;
}

.section-1 {
  background: rgba(255, 255, 255, 0.1);
  display: flex;
  justify-content: center;
}

@media only screen and (max-width: 1160px) {
  .what-is {
    flex-direction: column;
  }

  .section-text {
    display: flex;
    width: 100% !important;
  }

  .section-svg {
    display: flex;
    width: 90% !important;
    margin: 1rem auto;
  }
}
</style>
