<template>
    <section class="d-flex align-items-center text-center">
        <div class="container my-5">
            <h5 class="my-3">WE DO MORE FOR EVERYONE</h5>
            <h3>Action & <span class="highlighted-green">Projects</span></h3>
            <nav>
                <ul class="d-flex align-items-center justify-content-center">
                    <li class="nav-items p-3 m-3" v-for="(elem, index) in navItems" :key="index">{{elem}}</li>
                </ul>
            </nav>
        </div>

    </section>
</template>

<script>
    export default {
        name: 'ActionComp',
        data() {
            return {
                navItems: ['ALL', 'ISTITUTIONAL', 'SOCIAL', 'EVENTS', 'INNOVATION', 'ENVIRONMENT', 'TECHNOLOGY']
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
</style>