<template>
    <section class="container p-5 my-5">
        <div class="row">
            <div class="col-8">
                <h5>SEND A MESSAGE</h5>
                <h3>Get in <span class="highlighted-green">Touch</span></h3>
                <p>We will respond to your message as soon as possibile</p>
                <div class="container">
                    <form class="row">
                        <div class="col-6 py-4">
                            <div class="form-group">                               
                                <input type="text" class="form-control" v-model="InputName" placeholder="Name">
                            </div>
                        </div>
                        <div class="col-6 py-4">
                            <div class="form-group">                               
                                <input type="email" class="form-control" v-model="InputEmail" placeholder="Email">
                            </div>
                        </div>
                        <div class="col-6 py-4">
                            <div class="form-group">                               
                                <input type="text" class="form-control" v-model="InputPhone" placeholder="Phone">
                            </div>
                        </div>
                        <div class="col-6 py-4">
                            <select class="form-select" aria-label="Default select example">
                                <option selected>More Info</option>
                                <option value="1">One</option>
                                <option value="2">Two</option>
                                <option value="3">Three</option>
                            </select>                         
                        </div>

                        <div class="form-group p-0 py-4">                           
                            <textarea class="form-control" placeholder="Message" v-model="inputMessage" id="exampleFormControlTextarea1" rows="3"></textarea>
                        </div>
                    </form>

                    <button class="btn btn-green">SEND</button>
                    

                </div>
            </div>
            <div class="col-4">
                <h4>Example Inc.</h4>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>                
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
            <button class="btn btn-bg-white">VIEW MAP</button>
            </div>
        </div>

    </section>
</template>

<script>
    export default {
        name: 'FormComp'
    }
</script>

<style lang="scss" scoped>
@import '../style/style.scss';
.col-6{
    padding-left: 0;
    padding-right: 20px;
}

.btn{
    margin-left: -10px;
    margin-top: 20px;
}


.form-control, .form-select{
    background-color: #E9ECEF;
}

p{
    padding: 2px 0;
}

ul{
    color: #058283;
    font-size: 1.4rem;
    padding: 0;
    li{
        margin: 25px 0;
    }
    i{
        clip-path: circle();
        background-color: #d5e7e8;
        padding: 15px;
    }
}
</style>