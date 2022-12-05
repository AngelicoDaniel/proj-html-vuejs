<template>
    <div class="relative">
        <div class="top-bullets">
            <img src="../assets/img/bullets.png" alt="">
        </div>
        <div class="bottom-bullets">
            <img src="../assets/img/bullets.png" alt="">
        </div>
        <section>
            <div class="container-fluid">
                <div class="row h-100">
                    <div class="col-6 d-flex">
                    <div class="container w-50 m-auto">
                        <h5 class="py-2">ABOUT THE NETWORK</h5>
                        <h3><span class="highlighted-white">The</span> Company</h3>
                        <p>For 12 years we have been providing audit and warranty, financial advice, risk advice, taxes and related services to select clients.</p>
    
                        <div class="row">
                            <div v-for="(elem, index) in about" :key="index" class="col-6">
                                <h4><span><i :class="elem.icon" class="icons"></i></span>{{elem.title}}</h4>
                                <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit.</p>
                            </div>
                        </div>
                        <button class="btn-green">GET IN TOUCH</button>
                        <button class="btn-bg-none mx-5">READ MORE</button>
                    </div>
                    </div>
                    <div class="col-6">
                        <div class="about-img"></div>
                    </div>
                </div>
            </div>
        </section>
    </div>
</template>

<script>

    export default {
        name: 'AboutComp',
        data() {
            return {
                about: [
                    {
                      icon: "fas fa-ribbon",
                      title: "Tradition"
                    },
                    {
                      icon: "fas fa-lock",
                      title: "Security"
                    },
                    {
                      icon: "fas fa-edit",
                      title: "Certificate"
                    },
                    {
                      icon: "fas fa-graduation-cap",
                      title: "Expertise"
                    }
                ]
            }
        }
        
    }
</script>

<style lang="scss" scoped>
@import '../style/style.scss';
section{
    height: 90vh;
    background-color: #111117;
    color: white;
}
.relative{
    position: relative;
}
.top-bullets img{
    position: absolute;
    left: 46.4%;
    top: -5%;
    opacity: 0.3; 
    width: 9%;  
    aspect-ratio: 16/9;   
}
.bottom-bullets img{
    position: absolute;
    left: 46.4%;
    bottom: -5%;
    opacity: 0.3; 
    width: 9%;  
    aspect-ratio: 16/9;   
}
.about-img{
    background-image: url('../assets/img/about-4.jpg');
    height:90vh;
    object-fit: contain;
    
}
.icons{
    margin-right: 10px;
    font-size: 1.5rem;
    color: #058283;
}

</style>