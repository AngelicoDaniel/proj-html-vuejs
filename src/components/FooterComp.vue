<template>
    <section>
        <footer class="d-flex">
            <div class="w-75 m-auto d-flex align-items-center justify-content-between">
                <div class="col-3 m-3">
                    <div class="my-3">
                        <img src="../assets/img/logo.png" alt="">
                    </div>
                    <div>A Functional HTML Template for Corporate & Business.</div>
                    <ul>
                        <li>
                            <span><i class="fa-solid fa-phone"></i> +1 (305) 1234-5678</span> 
                        </li>
                        <li>
                            <span><i class="fa-solid fa-envelope"></i> hello@example.com</span>
                        </li>
                        <li>
                            <span><i class="fa-solid fa-location-dot"></i> Main Avenue, 987</span> 
                        </li>
                    </ul>
                    <button class="btn-bg-none">GET IN TOUCH</button>
                </div>
                <div v-for="(elem, index) in footerArr" :key="index" class="col-3 m-3 p-4">
                    <div class="footer-card">
                        <h4 class="text-white">{{elem.title}}</h4>
                        <ul>
                            <li>
                                <span><i class="fa-sharp fa-solid fa-chevron-right"></i> {{elem.li1}}</span>
                            </li>
                            <li>
                                <span><i class="fa-sharp fa-solid fa-chevron-right"></i> {{elem.li2}}</span>
                            </li>
                            <li>
                                <span><i class="fa-sharp fa-solid fa-chevron-right"></i> {{elem.li3}}</span>
                            </li>
                            <li>
                                <span><i class="fa-sharp fa-solid fa-chevron-right"></i> {{elem.li4}}</span>
                            </li>
                            <li>
                                <span><i class="fa-sharp fa-solid fa-chevron-right"></i> {{elem.li5}}</span>
                            </li>
                            <li>
                                <span><i class="fa-sharp fa-solid fa-chevron-right"></i> {{elem.li6}}</span>
                            </li>
                        </ul>

                    </div>
                </div>
            </div>
        </footer>                    
        <LastComp class="bottom-footer"/>
    </section>
</template>

<script>
import LastComp from './LastComp.vue'

    export default {
        name: 'FooterComp',
        components: {
            LastComp
        },
        data() {
            return {
                footerArr: [
                    {
                        title: 'About',
                        li1: 'The Company',
                        li2: 'Istitutional',
                        li3: 'Social & Events',
                        li4: 'Innovation',
                        li5: 'Environment',
                        li6: 'Technology'
                    },
                    {
                        title: 'Services',
                        li1: 'Audit & Assurance',
                        li2: 'Financial Advisory',
                        li3: 'Analytics M&A',
                        li4: 'Middle Marketing',
                        li5: 'Legal Consulting',
                        li6: 'Regulatory Risk'
                    },
                    {
                        title: 'Support',
                        li1: 'Responsibility',
                        li2: 'Terms of Use',
                        li3: 'About Coookies',
                        li4: 'Privacy Policy',
                        li5: 'Accessibility',
                        li6: 'Information'
                    }

                ]
            }
        }
    }
</script>

<style lang="scss" scoped>
@import '../style/style.scss';
footer{
    background-color: #111117;
    height: 50vh;
    color: #8c969b;
    
    img{
        height: 2.5rem;
        margin-left: 10px;
        // filter: invert(50%);
    }
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
}

.bottom-footer{
    height: 70px;
    background-color: black;
}
</style>