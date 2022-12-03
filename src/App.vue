<template>
  <div>
    <HeaderComp/>
    <JumboComp/>
    <BusinessAreas/>
    <MainComp/>
    <FooterComp/>
    

  </div>
</template>

<script>
import HeaderComp from './components/HeaderComp.vue'
import JumboComp from './components/JumboComp.vue'
import BusinessAreas from './components/BusinessAreas.vue'



import MainComp from './components/MainComp.vue'
import FooterComp from './components/FooterComp.vue'

export default {
  name: 'App',
  components: {
    HeaderComp,
    JumboComp,
    BusinessAreas,
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
