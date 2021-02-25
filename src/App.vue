<template>
  <div id="app">
    <div class="header">
      <div class="navbar">
        <div class="navbar-logo text-primary">SUBBED</div>
        <div class="navbar-routes">
          <span class="navbar-route">What is Subbed ?</span>
          <span class="navbar-route">How ?</span>
          <span class="navbar-route">Pricing</span>
          <button class="navbar-route-button button text-white bg-primary">Contact Us</button>
        </div>
      </div>
    </div>
    <Home />

  </div>
</template>

<script>
import Home from "./views/Home.vue";

export default {
  name: "App",
  components: {
    Home,
  },
};
</script>

<style>

@font-face {
  font-family: "NunitoSans";
  src: local("NunitoSans"), url(./fonts/NunitoSans/NunitoSans-Regular.ttf) format("truetype");
}




body {
  background: #000c1b;

  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-size: 16px ;
  font-family: NunitoSans !important;
  color:white;

}

.header{
  display: flex;
  justify-content: center;
}

.navbar {
  display: flex;
  color: white;
  justify-content: space-between;
  padding: 16px 8px;
  width: 1148px;
  height: 42px;
  align-items: center;

}

.navbar-logo{
  font-weight: 800;
  cursor: pointer;


}

.container{
  display:flex;
  max-width: 1148px;
}


.navbar-route{
  margin-right: 16px;
  cursor: pointer;
}

.button{
  padding: 8px 24px;
  outline: none;
  border:none;
  border-radius: 8px;
  cursor: pointer;
  font-size: 16px;
  line-height: 24px;
width: fit-content;
font-weight: 500;

}

.button:hover{
 box-shadow: 0 0 0.25rem #5f24d9;

}

.flex{
  display: flex;
}

.flex-col{
  flex-direction: column;
}

.justify-center{
  justify-content: center;
}

.align-items-center{
  align-items: center;
}

.text-center{
  text-align: center;
}

.text-white{
  color: white;
}

.text-black{
  color:black;
}

.text-primary{
  color:#5F24D9
}
.text-secondary{
  color:#50D38D
}

.text-danger{
  color:#FFD736
}

.text-safe{
  color:#89DBFF;
}

.bg-primary{
  background: #5F24D9;
}

.bg-secondary{
  background:#50D38D;

}

.bg-danger{
  background:#FFD736;

}

.bg-safe{
  background: #89DBFF;
}

.bg-white{
  background:white !important;

}

.bg-black{
  background: black;
}

.bg-transparent{
  background:transparent !important;

}

/*font-sizes */
.font-xs{
  font-size: 0.5rem;
}

.font-sm{
  font-size: 0.75rem;
}

.font-md{
  font-size: 1rem;
}
.font-lg{
  font-size: 1.5rem;
}

.font-xl{
  font-size: 2rem;
}

.font-xxl{
  font-size: 3rem;
}

/*font-weight */

.font-300{
  font-weight: 300;
}

.font-400{
  font-weight: 400;
}

.font-500{
  font-weight: 500;
}

.font-600{
  font-weight: 600;
}

.font-700{
  font-weight: 700;
}

.font-800{
  font-weight: 800;
}


/*margins */

.m-1{
  margin: 0.5rem;
}

.m-2{
  margin: 1rem;
}

.m-3{
  margin: 1.5rem;
}

.m-4{
  margin: 2rem;
}

.m-5{
  margin: 2.5rem;
}

.m-6{
  margin: 3rem;
}


.m-7{
  margin: 3.5rem;
}

.m-8{
  margin: 4rem;
}

.m-9{
  margin: 4.5rem;
}

.m-10{
  margin: 5rem;
}



.mt-1{
  margin-top: 0.5rem;
}

.mt-2{
  margin-top: 1rem;
}

.mt-3{
  margin-top: 1.5rem;
}

.mt-4{
  margin-top: 2rem;
}

.mt-5{
  margin-top: 2.5rem;
}

.mt-6{
  margin-top: 3rem;
}

.mt-7{
  margin-top: 3.5rem;
}

.mt-8{
  margin-top: 4rem;
}

.mt-9{
  margin-top: 4.5rem;
}

.mt-10{
  margin-top: 5rem;
}


.mr-1{
  margin-right: 0.5rem;
}

.mr-2{
  margin-right: 1rem;
}

.mr-3{
  margin-right: 1.5rem;
}

.mr-4{
  margin-right: 2rem;
}

.mr-5{
  margin-right: 2.5rem;
}

.mr-6{
  margin-right: 3rem;
}

.mr-7{
  margin-right: 3.5rem;
}

.mr-8{
  margin-right: 4rem;
}

.mr-9{
  margin-right: 4.5rem;
}

.mr-10{
  margin-right: 5rem;
}


.mb-1{
  margin-bottom: 0.5rem;
}

.mb-2{
  margin-bottom: 1rem;
}

.mb-3{
  margin-bottom: 1.5rem;
}

.mb-4{
  margin-bottom: 2rem;
}

.mb-5{
  margin-bottom: 2.5rem;
}

.mb-6{
  margin-bottom: 3rem;
}

.mb-7{
  margin-bottom: 3.5rem;
}

.mb-8{
  margin-bottom: 4rem;
}

.mb-9{
  margin-bottom: 4.5rem;
}

.mb-10{
  margin-bottom: 5rem;
}


.ml-1{
  margin-left: 0.5rem;
}

.ml-2{
  margin-left: 1rem;
}

.ml-3{
  margin-left: 1.5rem;
}

.ml-4{
  margin-left: 2rem;
}

.ml-5{
  margin-left: 2.5rem;
}

.ml-6{
  margin-left: 3rem;
}
.ml-7{
  margin-left: 3.5rem;
}

.ml-8{
  margin-left: 4rem;
}

.ml-9{
  margin-left: 4.5rem;
}

.ml-10{
  margin-left: 5rem;
}



.w-100{
  width: 100%;
}

.h-100{
  height: 100%;
}



.line {
  display: flex;
  width: 20px;
  margin: 0 8px;
    height: 4px;
        border-radius: 2px;
    
}

.input{
  height: 1rem;
  padding: 0.75rem;
  border-radius: 0.5rem;
  outline:none;
  border:none;
  width: 100%;
  }

  .input:focus{
    box-shadow:0 0  0 2px #5F24D9 ;
  }

  a{
    text-decoration: none;
  }


@media only screen and (max-width: 1160px) {
.navbar{
  width: 100%;
}
.navbar-route{
  display:none;
}

.container{
   max-width: 80%;
}

}

@media only screen and (max-width: 640px) {

.container{
   max-width: 90%;
}

}


</style>
