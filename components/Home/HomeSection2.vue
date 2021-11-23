<template>
  <div class="home__section2 pt-[120px] ">
    <div class="container">
      <div class="grid px-[40px]  pb-[50px] grid-cols-12">
        <div class="text-center col-span-12 md:col-start-3 md:col-span-8 ">
          <h2 class="text-[#aab0bc] font-bold">WHAT WE DO?</h2>
          <h3 class="text-[2.2rem] leading-[43px] mt-[15px] font-bold">The service we offer is specifically designed to meet your needs.</h3>
        </div>
      </div>

      <!-- <img src="~/static/images/icons/chat-2.svg"> -->
      <div class="grid gap-[20px] px-[40px] sm:grid-cols-1 md:grid-cols-2  xl:grid-cols-4">
          <div v-for="(item, index) in HomeCards" :key="index" >
            <div >
              <div class="bg-white shadow border rounded px-[40px] py-[40px] text-center">
               
                <img class="w-[52px] h-[52px] m-auto mb-[20px] " :src="require(`~/static/images/icons/${item.img}`)">
                  <h4 class="text-[17px] font-bold mb-[20px]">{{item.title}}</h4>
                  <p class="text-[#60697b] text-[17px] leading-[30px] mb-[10px]">{{item.textContent}}</p>
                  <a class="font-bold cursor-pointer more" :class="[item.class]">{{item.learnMore}}</a>
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
      HomeCards:[
        {
          img:'search-1.svg',
          title:'SEO Services',
          textContent:'Nulla vitae elit libero, a pharetra augue. Donec id elit non mi porta gravida at eget metus cras justo.',
          learnMore:'Learn More',
          class:'yellow'
        },
         {
          img:'browser.svg',
          title:'Web Design',
          textContent:'Nulla vitae elit libero, a pharetra augue. Donec id elit non mi porta gravida at eget metus cras justo.',
          learnMore:'Learn More',
          class:'red'
        },
         {
          img:'chat-2.svg',
          title:'Social Engagement',
          textContent:'Nulla vitae elit libero, a pharetra augue. Donec id elit non mi porta gravida at eget metus cras justo.',
          learnMore:'Learn More',
          class:'green'
        },
         {
          img:'megaphone.svg',
          title:'Content Marketing',
          textContent:'Nulla vitae elit libero, a pharetra augue. Donec id elit non mi porta gravida at eget metus cras justo.',
          learnMore:'Learn More',
          class:'blue'
        },
      ]
    }
  }
}
</script>

<style>
a.hover::before {
    content: "";
    transform-origin: 100% 50%;
    transform: scale3d(0,1,1);
    transition: transform .3s cubic-bezier(.7,0,.2,1);
}
a.hover::before {
    position: absolute;
    width: 100%;
    height: 1px;
    background: currentColor;
    top: 100%;
    left: 0;
    pointer-events: none;
}
a.hover {
    position: relative;
   
}
a {
    transition: all .2s ease-in-out;
}
.more:after {
    font-family: Font Awesome 5 Free;
    content: "\e902";
    padding-left: .05rem;
    font-size: .85rem;
    font-weight: 400;
    vertical-align: -2px;
    margin-right: -.25rem;
    display: inline-block;
}

</style>