<template>
  <div class="home_section8 bg-light angled upper-start lower-start">
    <div class="container">
      <div class="grid grid-cols-12 pb-[100px]  ">
        <div class="px-[40px] col-span-12 md:col-span-10 md:col-start-2 lg:col-span-7 " >
          <div class="grid grid-cols-12">
            <div class="col-span-12 p-[12px]  sm:col-span-6" v-for="(item, index) in steps" :key="index" :class="[{'lg:col-start-2':item.id == 3},{'lg:col-span-6': item.id % 2 == 0},{'lg:col-span-5': item.id % 2 != 0}]">
              <div :class="[`community_${item.id}`]" class="bg-white shadow-lg rounded-[10px] mt-[20px] p-[38px]">
           
                <div>
                  <p class="text-[17px] leading-[2rem]">{{item.textContent}}</p>
                  <h4 class="font-bold text-[1.2rem py-[10px]">{{item.title}}</h4>
                  <p> {{item.position}}</p>
                </div>
             
              </div>
            </div>
          </div>
        </div>

        <div class="px-[40px] col-span-12 m-auto md:col-span-10 md:col-start-2 lg:col-span-5 " >
          <h2 class="text-[#aab0bc] font-bold mb-[20px]">OUR COMMUNITY</h2> 
          <h3 class="text-[2.2rem] leading-[1.15] text-[#343f52]  font-bold">Don't take our word for it. See what customers are saying about us.</h3>
          
          <p class="text-[1.1rem] leading-[1.55] my-[35px] text-[#60697b] ">Aenean lacinia bibendum nulla sed consectetur. Praesent commodo cursus magna, vel scelerisque nisl consectetur et. Nulla vitae elit libero, 
            a pharetra augue. Maecenas faucibus mollis interdum. Vestibulum id ligula porta felis euismod.
          </p>
          <button class="bg-[#fab758] px-[24px] text-[1rem] py-[12px] text-white font-bold rounded-full  x ">
            All Testimonials </button>
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
          textContent:'“Cum sociis natoque penatibus et magnis dis parturient montes.”',
          title:'Coriss Ambady',
          position:'Financial Analyst',
          
        },
           {
          id:2,
          textContent:'“Vivamus sagittis lacus vel augue laoreet rutrum faucibus dolor auctor. Vestibulum id ligula porta felis euismod.”',
          title:'Cory Zamora',
          position:'Marketing Specialist',
          
        },
           {
          id:3,
          textContent:'“Donec id elit non porta gravida at eget metus. Duis mollis est luctus commodo nisi erat.”',
          title:'Barclay Widerski',
          position:'Sales Specialist',
          
        },
           {
          id:4,
          textContent:'“Nisi erat porttitor ligula, eget lacinia odio sem nec elit. Aenean eu leo pellentesque.”',
          title:'Jackie Sanders',
          position:'Investment Planner',
          
        },
        
       
      ]
    }
  }
}
</script>

<style>

</style>