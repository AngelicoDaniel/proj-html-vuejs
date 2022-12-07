<template>
    <div>                   
        <img :src="require(`../assets/img/project${dettagliCard.image}.jpg`)" alt="project">
        <div class="title col-8">{{dettagliCard.title}}</div>
        <div class="sub-title col-10">Lorem ipsum dolor sit amet consectetur, adipisicing elit</div>
    </div>
</template>

<script>
    export default {
        name: 'ActionCard',
        props: {
            dettagliCard: Array
        }
    }
</script>

<style lang="scss" scoped>
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
            left: 17%;
            color: white;
            font-weight: 600;
            font-size: 1.4rem;
            z-index: 10;
            
        }
        .sub-title{
            position: absolute;
            bottom: 40%;
            left: 10%;
            color: white;
            font-weight: 600;
            font-size: 1rem;
            z-index: 10;
            display: none;          
        }    
    
}
.card:hover {
            .sub-title{
                display: block;
            }           
        }
</style>