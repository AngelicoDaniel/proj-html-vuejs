<template>
    <section>
        <footer class="text-white d-flex">
            <div class="w-75 m-auto d-flex align-items-center">
                <div class="col-3 m-3">
                    <div>
                        <img src="../assets/img/logo.png" alt="">
                    </div>
                    <div>A Functional HTML Template for Corporate & Business.</div>
                    <ul>
                        <li>
                            <span class="green-circle"><i class="fa-solid fa-phone"></i> +1 (305) 1234-5678</span> 
                        </li>
                        <li>
                            <span class="green-circle"><i class="fa-solid fa-envelope"></i> hello@example.com</span>
                        </li>
                        <li>
                            <span class="green-circle"><i class="fa-solid fa-location-dot"></i> Main Avenue, 987</span> 
                        </li>
                    </ul>
                </div>
                <div class="col-3 m-3">lorem</div>
                <div class="col-3 m-3">lorem</div>
                <div class="col-3 m-3">lorem</div>
            </div>
        </footer>                    
        
    </section>
</template>

<script>
    export default {
        name: 'FooterComp'
    }
</script>

<style lang="scss" scoped>
@import '../style/style.scss';
footer{
    background-color: #111117;
    height: 50vh;
    img{
        height: 2.5rem;
        margin-left: 10px;
    }
}
</style>