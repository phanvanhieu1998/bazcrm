<template>
  
  <div class="home_section9 bg-light angled upper-end lower-end">
    <div class="container">
      <div class=" grid py-[20px] pt-[90px] grid-cols-12">
        <div class="px-[40px] pb-[20px]  col-span-12 md:col-span-10 md:col-start-2  lg:col-span-4 lg:pb-[0]"> 
          <h2 class="text-[#aab0bc] font-bold mb-[20px]">OUR PRICING</h2> 
          <h3 class="text-[2.2rem] leading-[1.15] text-[#343f52]  font-bold">We offer great and premium prices.</h3>
          <p class="text-[1rem] font-medium leading-[1.55] my-[35px] text-[#60697b] ">Enjoy a 
            <span class="text-[#fab758]">free 30-day trial </span>and experience the full service. No credit card required!</p>
           <button class="bg-[#fab758] px-[24px] text-[1rem] py-[12px] text-white font-bold rounded-full  x ">
            See All Prices </button>
        </div>

        <div class="px-[40px] col-span-12   md:col-span-10 md:col-start-2 lg:col-span-7 lg:col-start-6 ">
          <p class="flex md:justify-start   lg:justify-end font-semibold">Monthly
            <label class="switch mx-[20px]">
              <input type="checkbox">
              <span @click="b()" class="slider round"></span>
            </label>
            <span class="text-[#e2626b]">Yearly (Save 30%)</span>
          </p>

          <div class=" grid  grid-cols-12">
            <div v-for="(item, index) in pricing" :key="index" class="col-span-12  sm:px-[15px] sm:col-span-6 lg:col-span-6">
                <div class="bg-white px-[20px] shadow-lg rounded-[10px] mt-[20px] py-[40px] sm:px-[40px] m-auto lg:px-[50px]">
           
                <div >
                  <div :class="[{'price-show':package_term},{'price-hide':package_term == false}]" class="relative "><span class="font-semibold text-[25px] top-[17px] absolute ">$</span><span class="text-[3.6rem] font-semibold ml-[20px]">{{item.price}}</span>/ month</div>
                  <div :class="[{'price-show':package_term  == false},{'price-hide':package_term}]"  class="relative "><span class="font-semibold  text-[25px] top-[17px] absolute ">$</span><span class="text-[3.6rem] font-semibold ml-[20px]">{{item.priceYear}}</span>/ year</div>
                  <h4 class="text-[17px] text-[black] leading-[2rem] font-bold">{{item.title}}</h4>
                  <ul>
                    <li class="flex mt-[10px]">
                      <div>
                        <svg aria-hidden="true" focusable="false" data-prefix="fas" data-icon="check" class="inline-block svg-inline--fa fa-check fa-w-16 w-[13px] mr-[5px] h-[20px] text-[#fab758]" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512"><path fill="currentColor" d="M173.898 439.404l-166.4-166.4c-9.997-9.997-9.997-26.206 0-36.204l36.203-36.204c9.997-9.998 26.207-9.998 36.204 0L192 312.69 432.095 72.596c9.997-9.997 26.207-9.997 36.204 0l36.203 36.204c9.997 9.997 9.997 26.206 0 36.204l-294.4 294.401c-9.998 9.997-26.207 9.997-36.204-.001z"></path></svg>
                      </div> 
                      
                      <h2  class="font-bold ml-[5px]">{{item.projects}}</h2 >
                    </li>

                    <li class="flex mt-[10px]">
                      <div>
                        <svg aria-hidden="true" focusable="false" data-prefix="fas" data-icon="check" class="inline-block svg-inline--fa fa-check fa-w-16 w-[13px] mr-[5px] h-[20px] text-[#fab758]" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512"><path fill="currentColor" d="M173.898 439.404l-166.4-166.4c-9.997-9.997-9.997-26.206 0-36.204l36.203-36.204c9.997-9.998 26.207-9.998 36.204 0L192 312.69 432.095 72.596c9.997-9.997 26.207-9.997 36.204 0l36.203 36.204c9.997 9.997 9.997 26.206 0 36.204l-294.4 294.401c-9.998 9.997-26.207 9.997-36.204-.001z"></path></svg>
                      </div>
                      <h2 class="font-bold ml-[5px]" >{{item.access}} </h2 >
                    </li>

                    <li class="flex mt-[10px]">
                      <div>
                        <svg aria-hidden="true" focusable="false" data-prefix="fas" data-icon="check" class="inline-block svg-inline--fa fa-check fa-w-16 w-[13px] mr-[5px] h-[20px] text-[#fab758]" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512"><path fill="currentColor" d="M173.898 439.404l-166.4-166.4c-9.997-9.997-9.997-26.206 0-36.204l36.203-36.204c9.997-9.998 26.207-9.998 36.204 0L192 312.69 432.095 72.596c9.997-9.997 26.207-9.997 36.204 0l36.203 36.204c9.997 9.997 9.997 26.206 0 36.204l-294.4 294.401c-9.998 9.997-26.207 9.997-36.204-.001z"></path></svg>
                      </div>
                      <h2 class="font-bold ml-[5px]" >{{item.storage}}</h2 >
                    </li>

                    <li class="flex mt-[10px]">
                      <div>
                        <svg aria-hidden="true" focusable="false" data-prefix="fas" data-icon="check" class="inline-block svg-inline--fa fa-check fa-w-16 w-[13px] mr-[5px] h-[20px] text-[#fab758]" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512"><path fill="currentColor" d="M173.898 439.404l-166.4-166.4c-9.997-9.997-9.997-26.206 0-36.204l36.203-36.204c9.997-9.998 26.207-9.998 36.204 0L192 312.69 432.095 72.596c9.997-9.997 26.207-9.997 36.204 0l36.203 36.204c9.997 9.997 9.997 26.206 0 36.204l-294.4 294.401c-9.998 9.997-26.207 9.997-36.204-.001z"></path></svg>
                      </div>
                      <h2 class="font-bold ml-[5px]" > {{item.reports}}</h2 >
                    </li>

                    <li class="flex mt-[10px]">
                      <div>
                        <svg aria-hidden="true" focusable="false" data-prefix="fas" data-icon="check" class="inline-block svg-inline--fa fa-check fa-w-16 w-[13px] mr-[5px] h-[20px] text-[#fab758]" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512"><path fill="currentColor" d="M173.898 439.404l-166.4-166.4c-9.997-9.997-9.997-26.206 0-36.204l36.203-36.204c9.997-9.998 26.207-9.998 36.204 0L192 312.69 432.095 72.596c9.997-9.997 26.207-9.997 36.204 0l36.203 36.204c9.997 9.997 9.997 26.206 0 36.204l-294.4 294.401c-9.998 9.997-26.207 9.997-36.204-.001z"></path></svg>
                      </div>
                      <h2 class="font-bold ml-[5px]"> {{item.support}}</h2 >
                    </li>
                  </ul>
                </div>
                <button class="bg-[#fab758] px-[24px] text-[1rem] mt-[40px] py-[12px] text-white font-bold rounded-full  x ">
            Choose Plan </button>
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
     package_term:true,
     pricing:[
       {
         price:'19',
         priceYear:'199',
         title:'Premium Plan',
         projects:'5 Projects',
         access:'100k API Access',
         storage:'200MB Storage',
         reports:'Reports Weekly',
         support:'Support 7/24',
       },
           {
         price:'49',
         priceYear:'499',
         title:'Corporate Plan',
          projects:'5 Projects',
         access:'100k API Access',
         storage:'200MB Storage',
         reports:'Reports Weekly',
         support:'Support 7/24',
       },
     ]
   }
 },

 methods:{
   b(){
     this.package_term = !this.package_term
     console.log(this.a)
   }
 }


}
</script>

<style>
.switch {
  position: relative;
  display: inline-block;
  width: 50px;
  height: 25px;
}

.switch input { 
  opacity: 0;
  width: 0;
  height: 0;
}

.slider {
  position: absolute;
  cursor: pointer;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background-color: #eeeeef;
  -webkit-transition: .4s;
  transition: .4s;
}

.slider:before {
  position: absolute;
  content: "";
  height: 20px;
  width: 20px;

  left: 4px;
  bottom: 3px;
  background-color: #fab758;
  -webkit-transition: .4s;
  transition: .4s;
}

/* input:checked + .slider {
  background-color: #2196F3;
}

input:focus + .slider {
  box-shadow: 0 0 1px #2196F3;
} */

input:checked + .slider:before {
  -webkit-transform: translateX(22px);
  -ms-transform: translateX(22px);
  transform: translateX(22px);
}
.price-hide{
  /* animation: a 0.3s; */
   animation: b 1s forwards;
 
  
  display: none;
}
.price-show{
     animation: a 1s forwards;
      /* animation: b 1s forwards; */
     
}
/* Rounded sliders */
.slider.round {
  border-radius: 34px;
}

.slider.round:before {
  border-radius: 50%;
}
@keyframes a {
  0%{
    opacity: 0;
    transform: translateY(-80px);
  }
  100%{
    opacity: 1;
    transform: translateY(0px);
  }
}
@keyframes b {
  0%{
    opacity: 1;
    transform: translateY(0px);
  }
  100%{
    opacity: 0;
    transform: translateY(80px);
  }
}
</style>