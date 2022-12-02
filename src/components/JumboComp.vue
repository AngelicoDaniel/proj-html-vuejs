<template>
    <section>
        <img src="../assets/img/our-team.png" alt="bg-parralax" class="team">

        <div class="container w-50">
            <!-- logo -->
            <div class="row d-flex justify-between align-items-center py-3 m-auto">
                <div class="col-6">
                    <img class="nex" src="../assets/img/logo.png" alt="nex-gen-logo">
                </div>
            <!--nav-->
                <div class="col-6 d-flex justify-content-around">
                    <ul class="d-flex">
                        <li class="mx-2" v-for="(elem, index) in navItems" :key="index">{{elem}}</li>
                    </ul>
                </div>
            </div>

            <!--slogan-->
            <div class="h-100 d-flex flex-column align-items-center text-center my-5">
                <h1>Ready <span class="highlighted-green">Team</span></h1>
                <p class="p-3">
                    No matter what your company needs, we will be ready to assist you in the
                    best possible way.
                </p>
                <div class="d-flex">
                    <a href="#" class="btn btn-green">GET IN TOUCH</a>
                    <a href="#" class="btn btn-bg-white">READ MORE</a>
                </div>
            </div>
        </div>

    </section>
</template>

<script>
    export default {
        name: 'JumboComp',
        data() {
            return {
                navItems: ['HOME', 'SERVICES', 'ABOUT', 'PROJECTS', 'RESULTS', 'GET IN TOUCH']
            }
        }
    }
</script>

<style lang="scss" scoped>
section{
    background-image: url('../assets/img/squares.jpg');
    background-size: cover;
    background-repeat: no-repeat;
    position: relative;
    height: 95vh;
    white-space: nowrap;
    .team{
        position: absolute;
        top: -16%;
        left: 6%;
    }
    .nex{
        height: 60px;
    }
    a{
        text-decoration: none;
        margin: 20px;
    }
    .btn{
        padding: 0.5rem 1rem;
        border-radius: 2px;
        text-decoration: none;
        display: inline-block;
        flex-shrink: 0;
        cursor: pointer;
    }
    .highlighted-green{
        color: #058283;
        background-color: #d5e7e8;
        border-radius: 7px;
        padding-inline: 0.5rem;
        opacity: 0.8;
    }
    .btn-green{
        background-color: #058283;
        color: white;
    }
    .btn-bg-white{
        color: #058283;
        border: 1px solid #058283;
        background-color: white;
    }


}


</style>