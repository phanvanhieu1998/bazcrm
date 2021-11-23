<template>
  <div>
    <TheHeader />
    <Nuxt />
    <TheFooter />
  </div>
</template>

<script>
import TheHeader from '../components/Header.vue';
import TheFooter from '../components/Footer.vue';

export default {
  data() {
    return {
      
    }
  }, 

  components: {
    TheHeader,
    TheFooter
  }
}
</script>