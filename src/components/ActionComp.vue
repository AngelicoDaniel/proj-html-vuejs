<template>
    <section class="d-flex align-items-center text-center">
        <div class="container my-5">
            <h5 class="my-3">WE DO MORE FOR EVERYONE</h5>
            <h3>Action & <span class="highlighted-green">Projects</span></h3>
            <nav>
                <ul class="d-flex align-items-center justify-content-center">
                    <li class="nav-items p-3 m-2" v-for="(elem, index) in navItems" :key="index">{{elem}}</li>
                </ul>
            </nav>

            <div class="container-fluid">
                <div class="row justify-content-between">
                    <div v-for="(elem, index) in actionItems" :key="index" class="card container my-2">
                        <img :src="require(`../assets/img/project${elem.image}.jpg`)" alt="project">
                        <div class="title col-10 m-auto">{{elem.title}}</div>
                    </div>
                </div>
            </div>
        </div>

    </section>
</template>

<script>
    export default {
        name: 'ActionComp',
        data() {
            return {
                navItems: ['ALL', 'ISTITUTIONAL', 'SOCIAL', 'EVENTS', 'INNOVATION', 'ENVIRONMENT', 'TECHNOLOGY'],
                actionItems: [
                    {
                        image: "-1", 
                        title: "Academic professional program in social media",
                    },
                    {
                        image: "-2", 
                        title: "President's speech at the annual meeting",
                    },
                    {
                        image: "-3", 
                        title: "International business trip in Shanghai",
                    },
                    {
                        image: "-4", 
                        title: "Technology workshop with education theme",
                    },
                    {
                        image: "-5", 
                        title: "Donation of Clothes and food to the partner NGO",
                    },
                    {
                        image: "-6", 
                        title: "Confraternization of the procurement team",
                    },
                    

                ]
            }
        }
    }
</script>

<style lang="scss" scoped>
@import "../style/style.scss";
.nav-items{
    color: gray;
}
.nav-items:hover{
    border-radius: 2px;
    background-color: #d5e7e8;
    cursor: pointer;
}
.card{
    width: calc((100% / 3) - 40px);
    padding: 30px 20px;
    border: none;
    position: relative;
    img{
        filter:brightness(50%);
        border-radius: 20px;
    }
    
        .title{
            position: absolute;
            bottom: 20%;
            left: 10%;
            color: white;
            font-weight: 600;
            font-size: 1.4rem;
            z-index: 10;
            
        }
    
}
</style>