
<script>
export default {
    data() {
        return {
            yearMonth: false,
            choices:[
            

                 {title:'free',
                monthlyPrice:0,
                yearlyPrice:0,
                isPopular:false,

options:[
    {isAvaible:true,
    context:'50 Video minutes',
    },
     {isAvaible:true,
    context:'Up to 2 languages',
    },
     {isAvaible:false,
    context:'Other plan featuress',
    },
     {isAvaible:false,
    context:'Other plan features',
    },
     {isAvaible:false,
    context:'Other plan features',
    },
]

                },
                
                 {title:'junior',
                monthlyPrice:30,
                yearlyPrice:300,
                isPopular:false,
options:[
    {isAvaible:true,
    context:'50 Video minutes',
    },
     {isAvaible:true,
    context:'Up to 2 languages',
    },
     {isAvaible:true,
    context:'Other plan featuress',
    },
     {isAvaible:false,
    context:'Other plan features',
    },
     {isAvaible:false,
    context:'Other plan features',
    },
]

                },
                 {title:'explorer',
                monthlyPrice:50,
                yearlyPrice:500,
                isPopular:true,

options:[
    {isAvaible:true,
    context:'50 Video minutes',
    },
     {isAvaible:true,
    context:'Up to 2 languages',
    },
     {isAvaible:true,
    context:'Other plan featuress',
    },
     {isAvaible:true,
    context:'Other plan features',
    },
     {isAvaible:false,
    context:'Other plan features',
    },
]

                },

                 {title:'captain',
                monthlyPrice:0,
                yearlyPrice:0,
                isPopular:false,

options:[
    {isAvaible:true,
    context:'50 Video minutes',
    },
     {isAvaible:true,
    context:'Up to 2 languages',
    },
     {isAvaible:true,
    context:'Other plan featuress',
    },
     {isAvaible:true,
    context:'Other plan features',
    },
     {isAvaible:true,
    context:'Other plan features',
    },
]

                },
            ]
        }
    }
}
</script>

<template>
  <div class="section-5 container">

      
<div class="text-white font-xl font-800 text-center section-5-title"> 
      Our offers for in Platfom Service

</div>

<div class="flex section-5-buttons mt-3">

<button @click="yearMonth = false" :class="{'bg-white text-primary' : yearMonth == false}" class="section-5-button mr-1">Month</button>
<button @click="yearMonth = true" :class="{'bg-white' : yearMonth == true}" class="section-5-button">Year</button>

</div>

<div class="flex mt-10 section-5-choices">

<div  v-for="choice in choices" :key="choice">
<div :id="`${choice.title}`"  class="section-5-choice ">
<div class="section-5-choice-title font-xxl">{{choice.title.toUpperCase()}}</div>

<div class="section-5-choice-price align-items-center flex">$<span class="font-xxl ml-1 mr-1"> {{!yearMonth ? choice.monthlyPrice : choice.yearlyPrice }}</span> / {{!yearMonth ? 'Monthly' : 'Yearly'}}</div>
<div class=" section-5-choice-checks ">

    <div v-for="option in choice.options" :key="option" class="section-5-choice-check ">
            <img v-if="option.isAvaible" class="section-svg " src="../../assets/svg/double-check.svg" />
            <img v-else class="section-svg " src="../../assets/svg/times.svg" />

        {{option.context}}

</div>
</div>



    <button class="section-5-button2 bg-primary text-white mt-3 ">Try Now</button>

</div>

<span v-if="choice.isPopular" class="flex justify-center mt-3 font-800">Most Popular</span>


</div>

</div>

 <div class="flex">
<a class="section-5-choice-dots "    v-for="choice in choices" :key="choice" :href="`#${choice.title}`"></a>

 

 </div>
  </div>
</template>


<style scoped>

.section-5{
    display:flex;
    align-items: center;
    width: 100%;
    padding: 96px 0;

    flex-direction: column;
  
}


.section-5-button{
  padding: 4px 12px;
  outline: none;
  border:none;
  border-radius: 8px;
  cursor: pointer;
  font-size: 12px;
  line-height: 24px;
width: fit-content;
font-weight: 600;
background: transparent;

}

.section-5-buttons{
  padding: 8px;

  border-radius: 8px;
  cursor: pointer;

background: gray;

}



.section-5-button:hover{
 box-shadow: 0 0 0.25rem #5f24d9;

}

.section-5-choices{
    display:flex;
    width: 100%;
    justify-content: space-between;
}

.section-5-choice{
    border:2px solid #89DBFF;
    border-radius: 1rem;
    padding: 1.5rem;
    display:flex;
    flex-direction: column;
    width: 80%;
    justify-content: center;
    align-items: center;
}

.section-5-choice-title{
        background-color: #000c1b;
    background-image: linear-gradient(#89dbff,#4c6bff);
    background-clip: text;
  -webkit-text-fill-color: transparent;
}

.section-5-choice-checks{
    display:flex;
    width: 100%;
   flex-direction: column;
}

.section-5-choice-check{
    display:flex;
    width: 100%;
    justify-content: space-between;
   
}




    .section-5-button2{
  padding: 8px 24px;
  outline: none;
  border:none;
  border-radius: 8px;
  cursor: pointer;
  font-size: 24px;
width: fit-content;
font-weight: 500;
color: black;
    background: #89DBFF;
    width: 100%;


}

.section-5-button:hover{
 box-shadow: 0 0 0.25rem #5f24d9;

}

.section-5-choice-dots{
    background: #5f24d9;
    width: 40px;
    height: 40px;
    display:none;
    justify-content: center;
    align-items: center;
    border-radius: 50%;
margin:20px 20px;
}

@media only screen and (max-width: 1160px) {

.section-5-choices{
    display:flex;
    max-width: 100%;
    justify-content: space-between;
    overflow-x: auto;
    overflow-y:none !important;

     scroll-behavior: smooth;
-webkit-overflow-scrolling: touch;
}

.section-5-choice {
  width: 300px;
  flex-shrink: 0;
  margin: 0 16px;
  height: 80%;
}

.section-5-choice-check{
    display:flex;
    width: 100%;
    justify-content: flex-start;
   
}

.section-svg{
    width: 25px;
    height: 25px;
}

.section-5-choice-dots{
    display:flex;
}

.section-5-choice-dots:hover{
    display:flex;
    opacity: 0.2;
}

.section-5-choice-dots:active{
       opacity: 0.4;

}
}


</style>