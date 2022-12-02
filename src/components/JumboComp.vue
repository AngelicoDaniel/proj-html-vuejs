<template>
    <section>
        <img src="../assets/img/our-team.png" alt="bg-parralax" class="team">

    </section>
</template>

<script>
    export default {
        name: 'JumboComp'
    }
</script>

<style lang="scss" scoped>
section{
    background-image: url('../assets/img/squares.jpg');
    background-size: cover;
    background-repeat: no-repeat;
    position: relative;
    height: 95vh;
    .team{
        position: absolute;
        top: -16%;
        left: 6%;
      
    }
}


</style>