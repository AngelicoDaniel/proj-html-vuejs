<template>
    <div>
        <BusinessAreas/>
        <AboutComp/>
        <ActionComp/>
        <NumberComp/>
        <PartnersComp/>
        <FormComp/>
    </div>
</template>

<script>
import BusinessAreas from './BusinessAreas.vue'
import AboutComp from './AboutComp.vue'
import ActionComp from './ActionComp.vue'
import NumberComp from './NumberComp.vue'
import PartnersComp from './PartnersComp.vue'
import FormComp from './FormComp.vue'

    export default {
        name: 'MainComp',
        components: {
            BusinessAreas,
            AboutComp,
            ActionComp,
            NumberComp,
            PartnersComp,
            FormComp
        }
    }
</script>

<style lang="scss" scoped>

</style>