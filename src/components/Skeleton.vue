<template>
    <Navbar />
    <main>
        <slot></slot>
    </main>
</template>

<script>
import Navbar from './Navbar.vue'
export default {
    components: {
        Navbar,
    }

}
</script>

<style>
@import url("../styles/main.css");

body {
    scroll-snap-type: mandatory;
    background: linear-gradient(to bottom right,
            #d8aaaa,
            #b9b5e3,
            #7bd1b5,
            #dbdc7e,
            #eab791,
            #e5646a);
    overflow-x: hidden;
}
.row {
  display: flex;
}
.sp-btn {
  justify-content: space-between;
}
main {
  padding: 0em 2em;
}
@media only screen and (max-width:768px) {
    main{
        padding: 0em 1em;
    }
    
}
button{
    outline: none;
    padding: 0.3em;
    border-radius: 7px;
    border: none;
    cursor:pointer;
}
input{
    outline: none;
    border: 1.7px solid grey;
    padding: 0 1em;
}
.caption{
    font-size: 0.7em;
    color: grey;
}
</style>