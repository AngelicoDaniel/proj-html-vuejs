<template>
        <div>
            <div class="d-flex justify-content-between align-items-center m-2">
                <i :class="dettagliCard.icon"></i>
                <i class="fa-solid fa-arrow-right"></i>
            </div>
            <h4>{{dettagliCard.title}}</h4>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Blanditiis, soluta doloremque repellendus sunt</p>
        </div>
</template>

<script>
    export default {
        name: 'ServiceComp',
        props: {
            dettagliCard: Array
        }
    }
</script>

<style lang="scss" scoped>
i{
    font-size: 25px;
    color: #058283;
}

.fa-solid{
    padding: 8px;
    color: #82c1c1;
}
.fa-solid:hover{
    color: #058283;
    border-radius: 50%;
    background-color: #82c1c1;
}
</style>