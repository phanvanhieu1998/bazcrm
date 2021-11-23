<template>
  <div class="home__section5 mb-[10rem]">
    <div class="container">
      <div class=" grid  pt-[90px] grid-cols-12">
        <div class="px-[40px] m-auto col-span-10 col-start-2 lg:col-span-7">
          <img class="h-auto max-w-full object-cover" src="~/static/images/concept6.png">
        </div> 

        <div class=" px-[40px] pt-[40px]  col-span-12 md:col-span-10 md:col-start-2 lg:col-span-5 lg:pt-[0px] lg:text-left">  
          <h3 class="text-[#aab0bc]  font-bold  leading-[1.15]">WHY CHOOSE US?</h3>
          <h3 class="text-[1.8rem] my-[20px] font-bold text-[#343f52] leading-[1.55] lg:text-[2rem]  lg:my-[35px]">We bring solutions to make life easier for our clients.</h3>

          <div v-for="(item, index) in collapse" :key="index">
            <button class="collapsible text-[#343f52] text-[1.1rem] mb-[10px] font-bold hover:text-[#fab758]" @click="toggle(index)">{{item.title}}</button>

            <div class="content" ref="content">
              <p class="text-[#343f52] text-[1rem]">{{item.content}}</p>
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
      collapse:[
        {
          title:'Professional Design',
          content:'Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus. Cras mattis consectetur purus sit amet fermentum. Praesent commodo cursus magna, vel.'
        },
           {
          title:'Top-Notch Support',
          content:'Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus. Cras mattis consectetur purus sit amet fermentum. Praesent commodo cursus magna, vel.'
        },
           {
          title:'Header and Slide Option',
          content:'Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus. Cras mattis consectetur purus sit amet fermentum. Praesent commodo cursus magna, vel.'
        },
      ]
    }
  },

  methods: {
    toggle(index) {
      setTimeout(()=>{
        if(this.$refs.content[index].offsetHeight == 0){
          var x, i;
          x =  this.$refs.content;
          for (i = 0; i < x.length; i++) {  
            x[i].style.height = '0px';
          }
          this.$refs.content[index].style.height = this.$refs.content[index].scrollHeight + "px"
        }else{
          this.$refs.content[index].style.height = '0px'
        }
      },10)
    },
  },
}
</script>

<style>

.content {
  padding: 0 18px;
  height: 0;
  overflow: hidden;
  transition: height 0.2s ease-out;
 
}
</style>