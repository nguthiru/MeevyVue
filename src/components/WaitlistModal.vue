<template>
    <modal-vue @close="$emit('close')">
        <div class="modal-body">
            <div class="row">
                <i class="fa fa-clock"></i>
                <h3>Join Waitlist</h3>
            </div>
            <p>{{submitStatus}}</p>
            <div id="waitlist-form">
                <div class="form-container">
                    <label for="Email">Email Address</label>
                    <input type="email" placeholder="Your Email Address" v-model="email">
                </div>
                <div class="form-container">
                    <label for="Expectations">What do you expect</label>
                    <input type="text" placeholder="Tell us what you expect" v-model="info">
                </div>
            </div>
            <p class="caption">*We will email you in regards to your application</p>
            <button @click="submit">
                <div class="row">
                    <i class="fa fa-inbox"></i>
                    <p>Join Waitlist</p>
                </div>
            </button>
        </div>
    </modal-vue>
</template>

<script>
    import ModalVue from './base/Modal.vue';
    import axios from 'axios'
    export default {
        name: 'waitlist-modal',
        components:{
            ModalVue
        },
        data(){
            return {
                email: null,
                info: null,
                submitStatus:""
            }
        },
        methods:{
            async submit(){
                if(this.email!=null && this.info!=null){
                var res = await axios.post("https://souldate.herokuapp.com/public/waitlist/join/",{email:this.email,info:this.info})
                console.log(res.data)
                this.$emit('close');

            }
                else{
                    this.submitStatus = "Kindly fill all fields."
                }
            }
        }
    }
</script>

<style scoped>
    .row{
        justify-content: center;
        align-items: center;
    }
    .form-container{
        margin: 1.5em 0;
    }
    input{
        height: 40px;
        border-radius: 7px;
        width: 100%;
        min-width: 350px;
    }
    label{
        display: block;
        font-size: small;
        font-weight: 500;
    }
    button{
        color: white;
        background-color: black;
        padding: 0.8em 1.2em;
        width: 100%;
        text-align: center;
        display: flex;
        justify-content: center;
        align-items: center;
        margin: 1.5em 0;  
        
    }
  i{
        padding: 0 1.2em;

    }
</style>