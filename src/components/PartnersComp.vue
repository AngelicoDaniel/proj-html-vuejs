<template>
    <div>
        <div class="container">           
            <div v-for="(elem, index) in partners" :key="index">
                <img :src="require(`../assets/img/${elem.logo}`)" alt="partner-img">
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'PartnersComp',
        data() {
            return {
                partners: [
                    {
                        logo: 'logo-4.png'
                    },
                    {
                        logo: 'logo-5.png'
                    },
                    {
                        logo: 'logo-1.png'
                    },
                    {
                        logo: 'logo-2.png'
                    },
                    {
                        logo: 'logo-3.png'
                    },
                    {
                        logo: 'logo-4.png'
                    }
                ]
            }
        }
    }
</script>

<style lang="scss" scoped>
div{
    height: 200px;
    background-color: #111117;
    display: flex;
    justify-content: space-around;
    align-items: center;
    img{
        width: 100px;
        filter: brightness(4) invert(1);
    }

}
</style>