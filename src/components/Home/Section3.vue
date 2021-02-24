<template>
  <div class="what-is container">
    <img class="section-svg" src="../../assets/svg/section-3.svg" />

<div class="flex flex-col section-text">



<div class="text-white font-xl font-800"> 
How will Subbedd access my video and provide subtitling?
</div>

<div class="text-secondary font-sm flex align-items-center font-700 mt-3"> 
          <div class="line bg-secondary"></div>
Low-cost subtitling service </div>

<div class="mt-3 ">
If you already uploaded your content on any other video platform, just share the video link with us. Your video or channel will keep gaining followers and views on that platform via Subbedd.
</div>

<div class="mt-3 ">
We are getting so excited when getting new videos. Share your video via <span class="text-danger">[we need to provide a way of sending here]</span> with us and let us do the rest!</div>

<div class="flex align-items-center mt-3 subscribe">
    <input class="input mr-2" placeholder="example@mail.com" /> 
    <button class="button bg-primary text-white ">Contact Us</button>
    </div>

</div>

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
.subscribe{
    height: 40px;
}

.subscribe *{
    height: fit-content;
}

.subscribe input{
    width: 50%;
}

</style>