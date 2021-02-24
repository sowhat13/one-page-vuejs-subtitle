<script>
import Welcome from "../components/Home/Welcome.vue";
import Section1 from "../components/Home/Section1.vue";
import Section2 from "../components/Home/Section2.vue";
import Section3 from "../components/Home/Section3.vue";

import Section4 from "../components/Home/Section4.vue";




export default {
  name: "App",
  components: {
    Welcome,
    Section1,
    Section2,
    Section3,
    Section4,


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
<Section1  />
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

</div>
  </div>
</template>



<style scoped>
.home{
  display:flex;
  width: 100%;
  justify-content: center;
}

.home-container{
  display:block;
  width: 100%;
}

.section-0{

    display:flex;
    justify-content: center;
}

.section-1{

    background: rgba(255, 255, 255, 0.1);
    display:flex;
    justify-content: center;
}

</style>
