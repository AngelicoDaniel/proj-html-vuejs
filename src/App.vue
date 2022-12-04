<template>
  <div>
    <HeaderComp/>
    <JumboComp/>
    <BusinessAreas/>
    <AboutComp/>
    <ActionComp/>
    <NumberComp/>
    <PartnersComp/>
    <MainComp/>
    <FooterComp/>
    

  </div>
</template>

<script>
import HeaderComp from './components/HeaderComp.vue'
import JumboComp from './components/JumboComp.vue'
import BusinessAreas from './components/BusinessAreas.vue'
import AboutComp from './components/AboutComp.vue'
import ActionComp from './components/ActionComp.vue'
import NumberComp from './components/NumberComp.vue'
import PartnersComp from './components/PartnersComp.vue'



import MainComp from './components/MainComp.vue'
import FooterComp from './components/FooterComp.vue'

export default {
  name: 'App',
  components: {
    HeaderComp,
    JumboComp,
    BusinessAreas,
    AboutComp,
    ActionComp,
    NumberComp,
    PartnersComp,
    MainComp,
    FooterComp
  }
}
</script>

<style lang="scss">
@import "./style/style.scss";
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  list-style-type: none;
}
</style>
