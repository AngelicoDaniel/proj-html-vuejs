<template>
    <div>
        <div class="footer-card">
                <h4 class="text-white">{{dettagliCard.title}}</h4>
                <ul>
                    <li>
                        <span><i class="fa-sharp fa-solid fa-chevron-right"></i> {{dettagliCard.li1}}</span>
                    </li>
                    <li>
                        <span><i class="fa-sharp fa-solid fa-chevron-right"></i> {{dettagliCard.li2}}</span>
                    </li>
                    <li>
                        <span><i class="fa-sharp fa-solid fa-chevron-right"></i> {{dettagliCard.li3}}</span>
                    </li>
                    <li>
                        <span><i class="fa-sharp fa-solid fa-chevron-right"></i> {{dettagliCard.li4}}</span>
                    </li>
                    <li>
                        <span><i class="fa-sharp fa-solid fa-chevron-right"></i> {{dettagliCard.li5}}</span>
                    </li>
                    <li>
                        <span><i class="fa-sharp fa-solid fa-chevron-right"></i> {{dettagliCard.li6}}</span>
                    </li>
                </ul>

            </div>
    </div>
</template>

<script>
    export default {
        name: 'FooterCard',
        props: {
            dettagliCard: Array
        }
    }
</script>

<style lang="scss" scoped>
    ul{
        padding-left: 0;
        margin: 20px 0;
    }
    .fa-solid{
        margin: 10px 0;
    }
    .footer-card{
        background-color: #1d2023;
        padding: 40px;
        border-radius: 6%;
    }  
</style>