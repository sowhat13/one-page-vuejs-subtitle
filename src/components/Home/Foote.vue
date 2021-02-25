<template>
  <div class="what-is container  ">
<div class="footer-subscribe">
 <div class="flex flex-col">
<p class="font-700">
  Subscribe for the latest news and updates !
</p>

<small>
  Join 10.950 subscribers and get latest news and updates to your inbox each month.
</small>

<div class="flex align-items-center mt-3 subscribe">
    <input class="input mr-2" placeholder="example@mail.com" /> 
    <button class="button bg-black text-white ">Subscribe</button>
    </div>
 </div>

<img class="footer-svg" src="../../assets/svg/footerbanner.svg">
</div>

<div class="mt-6 pb-2 pt-2 footer-bottom">
          <div class="navbar-logo text-primary">SUBBED</div>

          <div class="footer-links flex"> 
            <a href="https://www.instagram.com/" target="_blank">
<img  src="../../assets/svg/instagrams.svg">

            
            </a>
             <a href="https://www.instagram.com/" target="_blank">
<img  src="../../assets/svg/instagrams.svg">

            
            </a>

          </div>

               <div class="footer-links-mobile"> 
            <a href="https://www.whatsapp.com/" target="_blank">
<img  src="../../assets/svg/whatsapp.svg">

            
            </a>
          

          </div>

          <div class="footer-label">
<img src="../../assets/lanista.png">

          </div>

</div>
  </div>
</template>



<style scoped>

.what-is{
    display:flex;
    justify-content: space-between;
    width: 100%;
       padding: 96px 0 0 0; 

       flex-direction: column;

  
}


.footer-subscribe{
  display:flex;
  border-radius: 16px;
  background: #5F24D9;
  padding: 2rem 4rem;
  align-items: center;
  justify-content: space-between;
}


.footer-bottom{
  display:flex;
justify-content: space-between;
height: 48px;
align-items: center;
}

.footer-label img{
  height: 36px !important;
}

.footer-links *{
 margin:0 4px;
}

.footer-links-mobile {
display:none;
}


.footer-links-mobile * {

 margin:0 4px;

}



@media only screen and (max-width: 1160px) {
.footer-svg{
  display:none;
}

.footer-links {
display:none;
}

.footer-links-mobile {
display:flex;
}


}
</style>