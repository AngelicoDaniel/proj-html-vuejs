<template>
    <div>
        <TopComp/>
        <JumboComp/>
    </div>
</template>

<script>
import TopComp from './TopComp.vue'
import JumboComp from './JumboComp.vue'

    export default {
        name: 'HeaderComp',
        components: {
            TopComp,
            JumboComp
        }
    }
</script>

<style lang="scss" scoped>

</style>