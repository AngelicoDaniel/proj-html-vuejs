<template>
    <section class="container">
        <div class="row align-items-center">
            <div class="col-8">
                <h5>SEND A MESSAGE</h5>
                <h3>Get in <span class="highlighted-green">Touch</span></h3>
                <p>We will respond to your message as soon as possibile</p>
                <div class="container">
                    <form class="row">
                        <div class="col-6">
                            <input type="text" v-model="InputName" placeholder="Name">
                        </div>
                        <div class="col-6">
                            <input type="email" v-model="InputEmail" placeholder="Email">
                        </div>
                        <div class="col-6">
                            <input type="number" v-model="inputPhone" placeholder="Phone">
                        </div>
                        <div class="col-6">
                            <select name="More info" id="">
                                <option value="opt-1">option 1</option>
                                <option value="opt-2">option 2</option>
                                <option value="opt-3">option 3</option>
                            </select>
                        </div>

                        <div class="col">
                            <input type="text-area" class="col-11 m-auto">
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
</style>