<template>
  <div class="what-is container">
    <img class="section-svg section-1-svg-1" src="../../assets/svg/section-1.svg" />

<div class="flex flex-col section-text">

<div class="text-secondary font-sm flex align-items-center font-700"> 
          <div class="line bg-secondary"></div>
Low-cost subtitling service </div>

<div class="text-white font-xl font-800 mt-3"> 
What is Subbedd ?
</div>


<span class="mt-3 ">
Subbedd is a low-cost, very accurate subtitling service. We use real translators to translate your videos for an affordable price. Most importantly, Subbedd is also a video browsing platform linking you with the rest of the world. You can be on Subbedd without even switching from a platform you already publish video in ! You just have to link it here and a click on Subbedd is a click on the platform you use !
    
</span>

<button class="button bg-primary text-white mt-3">Contact Us</button>

</div>

    <img class="section-svg section-1-svg-2" src="../../assets/svg/section-1.svg" />


  </div>
</template>

<script>
export default {

}
</script>

<style scoped>

.what-is{
    display:flex;
    justify-content: space-between;
    width: 100%;
       padding: 96px 0;

  
}

.section-svg{
    width: 45%;

}

.section-text{
    width: 45%;
}


.section-1-svg-2{
  display:none;

}



@media only screen and (max-width: 1160px) {
.what-is{
  flex-direction: column;
}

.section-text{
  display:flex;
  width: 100% !important;
}

.section-1-svg-1{
display: none;

}

.section-1-svg-2{
  display:flex;
  width: 90% !important;
  margin: 1rem auto;

}


}

</style>