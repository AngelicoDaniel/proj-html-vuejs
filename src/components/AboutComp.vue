<template>
    <section>
        <div class="container-fluid">
            <div class="row h-100">
                <div class="col-6 d-flex align-items-center">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Labore ab laboriosam voluptatibus aperiam eaque rem expedita itaque? Ratione quod doloremque minima corrupti beatae sed eius aliquid tempore mollitia voluptatum. Nemo.</div>
                <div class="col-6">
                    <div class="about-img"></div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
    export default {
        name: 'AboutComp'
        
    }
</script>

<style lang="scss" scoped>
@import '../style/style.scss';
section{
    height: 90vh;
    background-color: #111117;
    color: white;
}
.about-img{
    background-image: url('../assets/img/about-4.jpg');
    height:90vh;
    object-fit: contain;
    
}

</style>