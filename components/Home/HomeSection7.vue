<template>
  
  <div class="home__section7 pb-[10rem]">
    <div class="container">
      <div class=" grid  pt-[90px] grid-cols-12">
        <div class="px-[40px] pb-[20px]  m-auto col-span-12 md:col-span-10 md:col-start-2 lg:col-span-5 lg:pb-[0]"> 
          <h2 class="text-[#aab0bc] font-bold mb-[20px]">OUR SOLUTIONS</h2> 
          <h3 class="text-[2.2rem] leading-[1.15] text-[#343f52]  font-bold">We make your spending stress-free for you to have the perfect control.</h3>
          <p class="text-[1.2rem] leading-[1.55] my-[35px] text-[#60697b] ">Cum sociis natoque penatibus et magnis dis parturient montes,
             nascetur ridiculus mus. Cras justo odio, dapibus ac facilisis in, egestas eget quam. Praesent commodo cursus.</p>
        
          <div class="grid grid-cols-12">

            <div class="col-span-12 md:col-span-6">
              <div class="mb-[20px]" v-for="(item, index) in 2" :key="index">
                <div class="inline-block w-[20px] h-[20px] rounded-full bg-[#fef2e1] absolute">
                  <svg aria-hidden="true" focusable="false" data-prefix="fas" data-icon="check" class="m-auto svg-inline--fa fa-check fa-w-16 w-[10px] h-[20px] text-[#fab758]" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512"><path fill="currentColor" d="M173.898 439.404l-166.4-166.4c-9.997-9.997-9.997-26.206 0-36.204l36.203-36.204c9.997-9.998 26.207-9.998 36.204 0L192 312.69 432.095 72.596c9.997-9.997 26.207-9.997 36.204 0l36.203 36.204c9.997 9.997 9.997 26.206 0 36.204l-294.4 294.401c-9.998 9.997-26.207 9.997-36.204-.001z"></path></svg>
                </div>
                <div class="pl-[30px]">
                  Aenean quam ornare. Curabitur blandit.
                </div>
              </div>
            </div>

            <div class=" col-span-12 md:col-span-6">
              <div class="mb-[20px]" v-for="(item, index) in 2" :key="index">
                <div class="inline-block w-[20px] h-[20px] rounded-full bg-[#fef2e1] absolute">
                  <svg aria-hidden="true" focusable="false" data-prefix="fas" data-icon="check" class="m-auto svg-inline--fa fa-check fa-w-16 w-[10px] h-[20px] text-[#fab758]" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512"><path fill="currentColor" d="M173.898 439.404l-166.4-166.4c-9.997-9.997-9.997-26.206 0-36.204l36.203-36.204c9.997-9.998 26.207-9.998 36.204 0L192 312.69 432.095 72.596c9.997-9.997 26.207-9.997 36.204 0l36.203 36.204c9.997 9.997 9.997 26.206 0 36.204l-294.4 294.401c-9.998 9.997-26.207 9.997-36.204-.001z"></path></svg>
                </div>
                <div class="pl-[30px]">
                  Aenean quam ornare. Curabitur blandit.
                </div>
              </div>
            </div>
          </div>
        </div>


        <div class="px-[40px] col-span-12 m-auto md:col-span-10 md:col-start-2  lg:col-span-7">
          <img class="h-auto max-w-full object-cover" src="~/static/images/concept8.png">
        </div> 

     
      </div>
    </div>
  </div>
</template>

<script>


export default {
 data(){
   return{

   }
 }


}
</script>

<style>

</style>