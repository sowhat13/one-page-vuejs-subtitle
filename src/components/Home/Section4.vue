<template>
  <div class="what-is container">

<div class="flex flex-col section-text">



<div class="text-white font-xl font-800 flex align-items-center "> 
<div class="line bg-white"></div>What is Subbed ?
</div>

<div class="text-white flex flex-col align-items-center  mt-3"> 

<div class="section-4-texts">
<p>
    Subbedd is a low-cost, very accurate subtitling service. We use real translators to translate your videos for an affordable price.
</p>
<p>
Most importantly, Subbedd is also a video browsing platform linking you with the rest of the world. You can be on Subbedd without even switching from the platform you already publish video in ! You just have to link it here and a click on Subbedd is a click on the platform you use !
</p>

<a class="text-safe flex w-100  font-sm font-700" href="/pricing">See Pricing Options</a>

</div>


</div>



  </div>

  <div class="section-4-rightSide">
<div> 
    <div class="section-4-svg1-wrapper">
    <img class="section-4-svg1" src="../../assets/svg/dart.svg" />


    </div>


    <div class="text-white flex flex-col align-items-center  mt-3"> 

<div class="flex section-4-text-title font-800">
 No burden on your budget

</div>
<p class="flex w-100">

To reach talented creators with different budgets, our offers are far below the market price.</p>

</div>

    
     </div>


     <div> 
    <div class="section-4-svg2-wrapper">
    <img class="section-4-svg2" src="../../assets/svg/wallet.svg" />


    </div>


    <div class="text-white flex flex-col align-items-center  mt-3"> 

<div class="flex section-4-text-title font-800">
 No burden on your budget

</div>
<p class="flex w-100">
To reach talented creators with different budgets, our offers are far below the market price.</p>

</div>

    
     </div>


     <div> 
    <div class="section-4-svg3-wrapper">
    <img class="section-4-svg3" src="../../assets/svg/people.svg" />


    </div>


    <div class="text-white flex flex-col align-items-center  mt-3"> 

<div class="flex section-4-text-title font-800">
 No burden on your budget

</div>
<p class="flex w-100">

To reach talented creators with different budgets, our offers are far below the market price.</p>

</div>

    
     </div>


     <div> 
    <div class="section-4-svg4-wrapper">
    <img class="section-4-svg4" src="../../assets/svg/pacman.svg" />


    </div>


    <div class="text-white flex flex-col align-items-center  mt-3"> 

<div class="flex section-4-text-title font-800">
 No burden on your budget

</div>
<p class="flex w-100">

To reach talented creators with different budgets, our offers are far below the market price.</p>

</div>

    
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

.section-4-svg1-wrapper{
    background:#f4201138;
    border-radius: 50%;
    width: 64px;
    height: 64px;
   display:flex;
   justify-content: center;
   align-items: center;
}


.section-4-svg2-wrapper{
    background:#50d38d41;
    border-radius: 50%;
    width: 64px;
    height: 64px;
   display:flex;
   justify-content: center;
   align-items: center;
}


.section-4-svg3-wrapper{
    background:#ffd73650;
    border-radius: 50%;
    width: 64px;
    height: 64px;
   display:flex;
   justify-content: center;
   align-items: center;
}


.section-4-svg4-wrapper{
    background:#89dcff4f;
    border-radius: 50%;
    width: 64px;
    height: 64px;
   display:flex;
   justify-content: center;
   align-items: center;
}

.section-4-rightSide{
    display: grid;
    width: 50%;
     grid-template-columns: 1fr 1fr;
  grid-template-rows: 1fr 1fr;
  gap:1rem;
}




.section-text{
    width: 35%;
}


.section-4-text-title {
    width: 100%;
}






@media only screen and (max-width: 1160px) {
.section-4-texts{
    display:none;
}

.section-4-rightSide{
    display: flex;
    flex-direction: column;
        width: 100%;
 
}

.section-text{
    margin-left: 1rem;
}
}
</style>