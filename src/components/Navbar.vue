<template>
    <header class="row align-center">
        <router-link to="/">
            <img src="../assets/logo.png" alt="Meevy" id="home-logo" class='nav-logo'/>
            <img src="../assets/logo_small.png" alt="Meevy" id="home-logo-mobile" />
        </router-link>
        
        <ul class="nav-links row">
            
                <li class="nav-link"> <router-link to="/support/privacy">Your Privacy</router-link></li>
            
            <a href="#">
                <li class="nav-link"><router-link to="/support/terms">Terms Of Use</router-link></li>
            </a>
            <!-- <a href="#">
                <li class="nav-link">
                    <div class="dropdown col">
                        <div class="row" @click="supportDrop=!supportDrop">
                            Support
                            <i class="fa-solid fa-chevron-down"></i>
                        </div>
                        <div class="dropdown-items col" v-show="supportDrop">
                            
                            <router-link to="/support/privacy">Privacy Policy</router-link>
                            <router-link to="/support/terms">Terms & Conditions</router-link>
                           
                        </div>
                    </div>
                </li>
            </a> -->
        </ul>
        <WaitlistModal v-if="waitlistOpen" @close='waitlistOpen=false' @wheel.prevent @touchmove.prevent
            @scroll.prevent />
        <button @click="waitlistModal">
            Join Waitlist
        </button>
    </header>
</template>

<script>
import WaitlistModal from './WaitlistModal.vue';
export default {
    name: "navbar",
    data() {
        return {
            waitlistOpen: false,
            supportDrop: false
        }
    },
    methods: {
        waitlistModal() {
            window.scrollTo(0, 0)
            this.waitlistOpen = true;
        }
    },
    components: { WaitlistModal }
}
</script>

<style scoped>
#home-logo {
    width: 6em;
    height: 2em;
}
#home-logo-mobile{
    display: none;
}

header {
    padding: 1em;
    width: 100%;
    height: 8vh;
    position: fixed;
    top: 0;
    z-index: 100;
}
button {
    background-color: black;
    color: white;
    padding: 0.6em 1.2em
}

@media only screen and (max-width:768px) {
    header {
        font-size: small;
    }
    #home-logo{
        display: none;
    }
    #home-logo-mobile{
        display: block;
        height: 1.5em;
    }
    #features-link {
        display: none;
    }

    button {

        padding: 0.3em 0.6em
    }
}

header ul {
    flex-grow: 1;
    justify-content: center;
    align-items: center;
}

header a {
    color: inherit;
}

.row {
    align-items: center;
}

i {
    padding: 0 1em;
    cursor: pointer;
}

header ul .nav-link {
    padding: 0 1em;
    font-size: small;
    align-self: flex-start;
    position: relative;

}


.dropdown-items {
    position: absolute;
    top: 1.5em;
    background-color: white;
    padding: 1em;
    border-radius: 10px;
}

.col {
    flex-direction: column;
    display: flex;
}
a:hover{
    font-size: 1.05em;
}
.dropdown-items a {
    margin: 0.5em 0;

}
.router-link-active{
    font-weight: 600;
    display: block;
}
.router-link-active::after{
    content: '';
    display: block;
    width: 20px;
    height: 5px;
    background-color: black;
    margin: 0 auto;
    border-radius: 10px;
}
</style>