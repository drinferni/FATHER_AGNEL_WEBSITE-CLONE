<template>
  <headersTop></headersTop>
  <mainOne></mainOne>
  <mainTwo></mainTwo>
  <mainThree></mainThree>
  <mainFour></mainFour>
  <mainFive></mainFive>
  <mainSix></mainSix>
  
</template>

<script>
import headersTop from "./components/headers.vue"
import mainOne from "./components/main-1.vue"
import mainTwo from "./components/main-2.vue"
import mainThree from "./components/main-3.vue"
import mainFour from "./components/main-4.vue"
import mainFive from "./components/main-5.vue"
import mainSix from "./components/main-6.vue"
export default {
  name : "App" ,
  components : {
    headersTop,
    mainOne,
    mainTwo,
    mainThree,
    mainFour,
    mainFive,
    mainSix,
  },
  data () {
    return {
    }
  },
  
}

</script>

<style>

</style>