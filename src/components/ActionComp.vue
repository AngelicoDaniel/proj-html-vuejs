<template>
    <section class="d-flex align-items-center text-center my-5">
        <div class="container my-5">
            <h5 class="m-3">WE DO MORE FOR EVERYONE</h5>
            <h3>Action & <span class="highlighted-green">Projects</span></h3>
            <nav>
                <ul class="d-flex align-items-center justify-content-center">
                    <li class="nav-items p-3 m-2" v-for="(elem, index) in navItems" :key="index">{{elem}}</li>
                </ul>
            </nav>

            <div class="container-fluid">
                <div class="row justify-content-between">
                        <ActionCard v-for="(elem, index) in actionItems"
                        :key="index"
                        class="card container my-2"
                        :dettagliCard="elem"/>
                </div>
            </div>
        </div>

    </section>
</template>

<script>
import ActionCard from './ActionCard.vue'
    export default {
        name: 'ActionComp',
        components: {
            ActionCard,
        },
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
h5{
    margin-left: 20px;
}
.nav-items{
    color: gray;
}
.nav-items:hover{
    border-radius: 2px;
    background-color: #d5e7e8;
    cursor: pointer;
}

</style>