<template>
    <section>
        <div class="container">
            <div>
                <div>
                    <h5 class="py-3">OUR BUSINESS AREAS</h5>
                    <h3>Excellence in <span class="highlighted-green">Services</span></h3>
                    <div class="d-flex justify-content-between align-items-center">
                        <p class="py-2 col-8 my-3">We are leaders in providing consultancy services with a set of cutting-edge technologies and a team of experienced and renowed professionals. These are some options that you can hire.</p>
                        <button href="#" class="btn-green">READ MORE</button>                  
                    </div>                    
                </div>
            </div>

            <!--services-->
            <div class="services">
                <div class="card">
                    <div class="d-flex justify-content-between">
                        <i>lorem</i>
                        <i>lorem</i>
                    </div>
                    <h4>Aduit e asscurance</h4>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Blanditiis, soluta doloremque repellendus sunt</p>
                </div>
            </div>

        </div>

    </section>
</template>

<script>
    export default {
        name: 'BusinessAreas'
    }
</script>

<style lang="scss" scoped>
@import "../style/style.scss";

section{
    background-color: #EEf4ED;
    padding: 20px;
}

.services{
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    align-items: center;
}

.card{
    width: calc(100% / 3);
}
</style>