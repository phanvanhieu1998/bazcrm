<template>
  <div class="home_section4 bg-light angled upper-start lower-start">
    <div class="container">
      <div class="grid grid-cols-12">
        <div class="px-[40px] col-span-12 md:col-span-10 md:col-start-2 lg:col-span-6 " >
          <h2 class="text-[#aab0bc] font-bold mb-[20px]">OUR STRATEGY</h2> 
          <h3 class="text-[2.2rem] leading-[1.15] text-[#343f52]  font-bold">Here are 3 working steps to organize our business projects.</h3>
           <p class="text-[1.2rem] leading-[1.55] my-[35px] text-[#60697b] ">Aenean eu leo quam. Pellentesque ornare sem lacinia quam venenatis vestibulum.
              Etiam porta sem malesuada magna mollis euismod. Nullam id dolor id nibh ultricies vehicula ut id elit. Nullam quis risus eget urna mollis.</p>
          <p class="text-[1.2rem] leading-[1.55] my-[35px] text-[#60697b] ">Nullam id dolor id nibh ultricies vehicula ut id elit.
             Vestibulum id ligula porta felis euismod semper. Aenean lacinia bibendum nulla sed consectetur.</p>
          <button class="bg-[#fab758] px-[24px] text-[1rem] py-[12px] text-white font-bold rounded-full  x ">
            Learn More </button>
        </div>

        <div class="px-[40px] col-span-12 md:col-span-10 md:col-start-2 lg:col-span-6 " >
          <div v-for="(item, index) in steps" :key="index">
            <div :class="[`step_${item.id}`]" class="bg-white shadow-lg rounded-[10px] mt-[20px] p-[38px]">
              <div class="flex ">
                <div class="w-[3.5rem] h-[3.5rem] bg-[#fef3e4] mr-[20px] rounded-full flex justify-center items-center font-bold text-[#fab758]">
                    {{item.step}}
                </div>
                  
                <div>
                    <h4 class="font-bold text-[1.4rem]">{{item.title}}</h4>
                  <p class="text-[17px]">{{item.textContent}}</p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data(){
    return{
      steps:[
        {
          id:1,
          step:'01',
          title:'Collect Ideas',
          textContent:'Nulla vitae elit libero pharetra augue dapibus.'
        },
         {
          id:2,
          step:'02',
          title:'Data Analysis',
          textContent:'Vivamus sagittis lacus vel augue laoreet.'
        },
         {
           id:3,
          step:'03',
          title:'Finalize Product',
          textContent:'Cras mattis consectetur purus sit amet.'
        },
       
      ]
    }
  }
}
</script>

<style>

</style>