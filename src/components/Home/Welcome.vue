<script>
export default {

    data(){
        return{
            isVideoPlaying: false,
        }
    },

mounted(){

    
function labnolIframe(div) {
       document.getElementById("videoPlayButton").setAttribute("style", "display:none");


  var iframe = document.createElement("iframe");
   iframe.setAttribute("style", "width:100%; border-radius:16px");


  iframe.setAttribute(
    "src",
    "https://www.youtube.com/embed/" + div.dataset.id + "?autoplay=1&rel=0"
  );
  iframe.setAttribute("frameborder", "0");
  iframe.setAttribute("allowfullscreen", "1");
  iframe.setAttribute(
    "allow",
    "accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture"
  );

  div.parentNode.replaceChild(iframe, div);
}

function initYouTubeVideos() {
  var playerElements = document.getElementsByClassName("youtube-player");
  for (var n = 0; n < playerElements.length; n++) {
    var videoId = playerElements[n].dataset.id;
    var div = document.createElement("div");
    div.setAttribute("data-id", videoId);
    div.setAttribute("style", "width:100%; border-radius:16px");

   

    var thumbNode = document.createElement("img");
   thumbNode.setAttribute("style", "width:100%; height:322px; border-radius:16px; object-fit:cover;");


    thumbNode.src = "https://i.ytimg.com/vi/ID/hqdefault.jpg".replace(
      "ID",
      videoId
    );


   


    div.appendChild(thumbNode);


   
    div.onclick = function () {


      labnolIframe(this);
    };
    playerElements[n].appendChild(div);
  }
}


document.addEventListener("DOMContentLoaded", initYouTubeVideos);


    
}



};


</script>


<template>
  <div class="welcome container">
      <span class="mt-6 font-md font-800 flex justify-center text-secondary text-center">
DISCOVER THE WORLD FOR FREE !

      </span>

      <span class="mt-3 font-xl font-800 flex justify-center text-center">

          Browse videos globally to watch in your language.
      </span>

<div class=" mt-10 tv-units">

    <div class="tv-1">
   <div class="grid-container">
<div class="small-tv1 small-tv">
    <img src="../../assets/svg/small-tv.svg" />

</div>
  <div class="small-tv2 small-tv">
    <img src="../../assets/svg/small-tv.svg" />
      

  </div>
  <div class="normal-tv ">
<div class="tv-gif1"></div>
    <img class="normal-tv-wrap" src="../../assets/svg/normal-tv-yellow.svg" />


  </div>


    </div>


       <div class="grid-container2 mt-1">
<div class="small-tv1 small-tv">
    <img src="../../assets/svg/small-tv.svg" />

</div>
  <div class="small-tv2 small-tv">
    <img src="../../assets/svg/small-tv.svg" />
      

  </div>
  <div class="normal-tv ">
<div class="tv-gif2"></div>

       <img class="normal-tv-wrap" src="../../assets/svg/normal-tv-blue.svg" />



  </div>


    </div>



    </div>

 <div class="tv-2" id="main">
  <div  class="youtube-player" data-id="8qIKZfHQ-3Q" />
  <div id="videoPlayButton"  class="video-play-button"></div>
</div>




    <div class="tv-3">
   <div class="grid-container">
<div class="small-tv1 small-tv">
    <img src="../../assets/svg/small-tv.svg" />

</div>
  <div class="small-tv2 small-tv">
    <img src="../../assets/svg/small-tv.svg" />
      

  </div>
  <div class="normal-tv ">
<div class="tv-gif3"></div>

        <img class="normal-tv-wrap" src="../../assets/svg/normal-tv-blue.svg" />


  </div>


    </div>


       <div class="grid-container2 mt-1">
<div class="small-tv1 small-tv">
    <img src="../../assets/svg/small-tv.svg" />

</div>
  <div class="small-tv2 small-tv">
    <img src="../../assets/svg/small-tv.svg" />
      

  </div>
  <div class="normal-tv ">
<div class="tv-gif4"></div>

    <img class="normal-tv-wrap" src="../../assets/svg/normal-tv-yellow.svg" />



  </div>


    </div>


</div>

    </div>

    <img class="subtitle-suprise" src="../../assets/svg/subtitlesuprise.svg" />
    

  </div>
</template>



<style scoped>

.welcome{
    display:flex;
    justify-content: center;
    flex-direction: column;
    width: 100%;
    padding-bottom: 80px;
}

.tv-units{
display: grid;
grid-template-columns: 25% 50% 25%;

}

.tv-2{
    position: relative;

    display:flex;
    width: 100%;
    padding: 8px 0px;

}

.youtube-player{
    display:flex;
    padding: 0 16px;
    width: 100%;
  cursor: pointer;

}

 .video-play-button {
  height: 72px;
  width: 72px;
 
top: calc(50% - 36px);
left:calc(50% - 36px);

  position: absolute;
  background: url("https://i.imgur.com/TxzC70f.png") no-repeat;
  cursor: pointer;
}


.grid-container {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  grid-template-rows: 1fr 1fr;
  gap: 16px 16px;
  grid-template-areas:
    "small-tv1 normal-tv normal-tv"
    "small-tv2 normal-tv normal-tv";
}

.grid-container2 {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  grid-template-rows: 1fr 1fr;
  gap: 16px 16px;
  grid-template-areas:
    "normal-tv normal-tv small-tv1"
    "normal-tv normal-tv small-tv2";
}

.small-tv{
    width: 81px;
    height: 71px;
}

.small-tv1 { grid-area: small-tv1; }

.small-tv2 { grid-area: small-tv2; }

.normal-tv { grid-area: normal-tv; 
position: relative;

}

.normal-tv-wrap{
  position: absolute;
z-index: 1;

}

.subtitle-suprise{
    width: 272px;
    position: relative;
    left: 50%;
}

.tv-gif1{
  background:url('https://media.giphy.com/media/QIabLW8w6BWU1RTqd3/giphy.gif');
  background-repeat: no-repeat;
  width: 182px ;
  height: 120px;
  position: absolute;
  background-size: cover;
z-index: 0;
  border-radius: 16px;

}

.tv-gif2{
    background:url('https://media.giphy.com/media/qJzPR90fB8qod6mWxJ/giphy.gif');
  background-repeat: no-repeat;
  width: 182px ;
  height: 120px;
  position: absolute;
  background-size: cover;
z-index: 0;
  border-radius: 16px;

}

.tv-gif3{
  background:url('https://media.giphy.com/media/eceAfd3KL993GCsayo/giphy.gif');
  background-repeat: no-repeat;
  width: 182px ;
  height: 120px;
  position: absolute;
  background-size: cover;
z-index: 0;
  border-radius: 16px;

}

.tv-gif4{
  background:url('https://media.giphy.com/media/4tBjRTBDV2f1JKrJVD/giphy.gif');
   background-repeat: no-repeat;
  width: 182px ;
  height: 120px;
  position: absolute;
  background-size: cover;
z-index: 0;
  border-radius: 16px;
}


@media only screen and (max-width: 1160px) {
.tv-units{
display: flex;
justify-content: center;
}

.tv-1{
  display:none;
}

.tv-2{
width: 90%;
min-width: 320px;

}

.tv-3{
  display:none;
}

.subtitle-suprise{
    width: 250px;
    position: relative;
    left: 25%;
}

}

@media only screen and (max-width: 640px) {
.tv-units{
display: flex;
justify-content: center;
}


.tv-2{
width: 100%;
min-width: 320px;

}


.youtube-player{
    padding: 0 ;
 

}

.subtitle-suprise{
    width: 250px;
    position: relative;
    left: 25%;
}

}
</style>