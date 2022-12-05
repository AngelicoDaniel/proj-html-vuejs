<template>
    <section class="container my-5">
        <div class="row align-items-center">
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

                        <div class="form-group p-0">                           
                            <textarea class="form-control" placeholder="Message" v-model="inputMessage" id="exampleFormControlTextarea1" rows="3"></textarea>
                        </div>
                    </form>
                    

                </div>
            </div>
            <div class="col-4">Lorem ipsum dolor sit amet consectetur, adipisicing elit. Consequuntur consectetur totam illo voluptatum! Et eos ad dolore fugiat unde, quia veritatis molestias doloremque nam, aliquid eveniet aperiam sit quae ut.</div>
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

.form-control, .form-select{
    background-color: #E9ECEF;
}
</style>