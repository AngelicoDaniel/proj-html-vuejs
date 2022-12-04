<template>
    <section>
        <h5 class="py-5">WHAT ARE WE DOING</h5>
        <h3 class="text-white"><span class="highlighted-white">Results</span> in Numbers</h3>

        <ul class="d-flex justify-content-around align-items-center text-white my-5 py-5">
            <li v-for="(elem, index) in arrNumbers" :key="index" >
                <div class="number">{{elem.number}}</div>
                <h2>{{elem.object}}</h2>
            </li>
        </ul>
    </section>
</template>

<script>
    export default {
        name: 'NumberComp',
        data() {
            return {
                arrNumbers: [
                    {
                        number: '128',
                        object: 'Certifications'
                    },
                    {
                        number: '230',
                        object: 'Employess'
                    },
                    {
                        number: '517',
                        object: 'Customers'
                    },
                    {
                        number: '94',
                        object: 'Countries Served'
                    },
                ]
            }
        }
        
    }
</script>

<style lang="scss" scoped>
@import '../style/style.scss';
section{
    height: 500px;
    background-image: url('../assets/img/bg-7.jpg');
    background-repeat: no-repeat;
    background-position: center;
    text-align: center;
    // display: flex;
    // flex-direction: column;
    // align-items: center;
    // justify-content: space-around;

    .number{
        color: #058283;
        font-size: 2rem;
        font-weight: 700;
    }
    
}

</style>