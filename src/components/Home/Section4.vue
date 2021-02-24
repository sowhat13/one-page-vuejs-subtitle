
<script>
export default {
    data() {
        return {
            yearMonth: false,
            choices:[
            

                 {title:'free',
                monthlyPrice:0,
                yearlyPrice:0,
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
  <div class="section-4 container">

      
<div class="text-white font-xl font-800"> 
      Our offers for in Platfom Service

</div>

<div class="flex section-4-buttons mt-3">

<button @click="yearMonth = false" :class="{'bg-white text-primary' : yearMonth == false}" class="section-4-button mr-1">Month</button>
<button @click="yearMonth = true" :class="{'bg-white' : yearMonth == true}" class="section-4-button">Year</button>

</div>

<div class="flex mt-10 section-4-choices">

<div v-for="choice in choices" :key="choice" class="section-4-choice">
<div class="section-4-choice-title font-xxl">{{choice.title.toUpperCase()}}</div>

<div class="section-4-choice-price align-items-center flex">$<span class="font-xxl ml-1 mr-1"> {{!yearMonth ? choice.monthlyPrice : choice.yearlyPrice }}</span> / {{!yearMonth ? 'Monthly' : 'Yearly'}}</div>
<div class="flex flex-col">

    <div v-for="option in choice.options" :key="option" class="section-4-choice-check flex">
            <img v-if="option.isAvaible" class="section-svg mr-3" src="../../assets/svg/double-check.svg" />
            <img v-else class="section-svg mr-3" src="../../assets/svg/times.svg" />

        {{option.context}}

</div>
</div>



    <button class="section-4-button2 bg-primary text-white mt-3 ">Try Now</button>

</div>



</div>


  </div>
</template>


<style scoped>

.section-4{
    display:flex;
    align-items: center;
    width: 100%;
    padding: 96px 0;

    flex-direction: column;
  
}


.section-4-button{
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

.section-4-buttons{
  padding: 8px;

  border-radius: 8px;
  cursor: pointer;

background: gray;

}


.section-4-button:hover{
 box-shadow: 0 0 0.25rem #5f24d9;

}

.section-4-choices{
    display:flex;
    width: 100%;
    justify-content: space-between;
}

.section-4-choice{
    border:2px solid #89DBFF;
    border-radius: 1rem;
    padding: 1.5rem;
    display:flex;
    flex-direction: column;
    width: 19%;
    justify-content: center;
    align-items: center;
}

.section-4-choice-title{
        background-color: #000c1b;
    background-image: linear-gradient(#89dbff,#4c6bff);
    background-clip: text;
  -webkit-text-fill-color: transparent;
}

.section-4-choice-check{
    display:flex;
    width: 100%;
   
}




    .section-4-button2{
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

.section-4-button:hover{
 box-shadow: 0 0 0.25rem #5f24d9;

}

</style>