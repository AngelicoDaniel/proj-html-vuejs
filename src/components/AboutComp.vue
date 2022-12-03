<template>
    <section>
        <div class="container-fluid">
            <div class="row h-100">
                <div class="col-6 d-flex">
                <div class="container w-50 m-auto">
                    <h5 class="py-2">ABOUT THE NETWORK</h5>
                    <h3><span class="highlighted-white">The</span> Company</h3>
                    <p>For 12 years we have been providing audit and warranty, financial advice, risk advice, taxes and related services to select clients.</p>

                    <div class="row">
                        <div class="col-6">
                            Lorem ipsum dolor sit amet consectetur, adipisicing elit. Atque vel incidunt, iusto consectetur dolore, alias esse facere blanditiis voluptatum minus adipisci nemo voluptate unde, quia exercitationem cumque nostrum. Necessitatibus, animi.
                        </div>
                        <div class="col-6">
                            Lorem ipsum dolor sit amet consectetur, adipisicing elit. Atque vel incidunt, iusto consectetur dolore, alias esse facere blanditiis voluptatum minus adipisci nemo voluptate unde, quia exercitationem cumque nostrum. Necessitatibus, animi.
                        </div>
                        <div class="col-6">
                            Lorem ipsum dolor sit amet consectetur, adipisicing elit. Atque vel incidunt, iusto consectetur dolore, alias esse facere blanditiis voluptatum minus adipisci nemo voluptate unde, quia exercitationem cumque nostrum. Necessitatibus, animi.
                        </div>
                        <div class="col-6">
                            Lorem ipsum dolor sit amet consectetur, adipisicing elit. Atque vel incidunt, iusto consectetur dolore, alias esse facere blanditiis voluptatum minus adipisci nemo voluptate unde, quia exercitationem cumque nostrum. Necessitatibus, animi.
                        </div>
                    </div>
                    <button>GET IN TOUCH</button>
                    <button>READ MORE</button>
                </div>
                </div>
                <div class="col-6">
                    <div class="about-img"></div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
    export default {
        name: 'AboutComp'
        
    }
</script>

<style lang="scss" scoped>
@import '../style/style.scss';
section{
    height: 90vh;
    background-color: #111117;
    color: white;
}
.about-img{
    background-image: url('../assets/img/about-4.jpg');
    height:90vh;
    object-fit: contain;
    
}

</style>