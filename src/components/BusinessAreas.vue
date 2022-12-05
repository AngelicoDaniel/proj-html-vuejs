<template>
    <section>
        <div class="container my-5">
            <div>
                <div>
                    <h5 class="py-4">OUR BUSINESS AREAS</h5>
                    <h3>Excellence in <span class="highlighted-green">Services</span></h3>
                    <div class="d-flex justify-content-between align-items-center">
                        <p class="py-2 col-8 my-3">We are leaders in providing consultancy services with a set of cutting-edge technologies and a team of experienced and renowed professionals. These are some options that you can hire.</p>
                        <button href="#" class="btn-green">READ MORE</button>                  
                    </div>                    
                </div>
            </div>

            <!--services-->
            <div class="services container-fluid">
                <div class="row justify-content-between">
                    <div v-for="(service, index) in services" :key="index" class="card my-4">
                        <div class="d-flex justify-content-between align-items-center m-2">
                            <i :class="service.icon"></i>
                            <i class="fa-solid fa-arrow-right"></i>
                        </div>
                        <h4>{{service.title}}</h4>
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Blanditiis, soluta doloremque repellendus sunt</p>
                    </div>
                </div>
            </div>

        </div>

    </section>
</template>

<script>
    export default {
        name: 'BusinessAreas',
        data() {
            return {
                services: [
                    {
                        icon: "fas fa-network-wired", 
                        title: "Audit & Insurance",
                    },
                    {
                        icon: "fas fa-briefcase", 
                        title: "Financial Advisory",
                    },
                    {
                        icon: "far fa-chart-bar", 
                        title: "Analytics and M&A",
                    },
                    {
                        icon: "fas fa-rocket", 
                        title: "Middle Marketing",
                    },
                    {
                        icon: "fas fa-globe", 
                        title: "Legal Consulting",
                    },
                    {
                        icon: "fas fa-inbox", 
                        title: "Regulatory Risk",
                    },
                    

                ]
            }
        }
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
    width: calc((100% / 3) - 40px);
    padding: 30px 20px;
    border: none;
}

i{
    font-size: 25px;
    color: #82c1c1;
}
</style>