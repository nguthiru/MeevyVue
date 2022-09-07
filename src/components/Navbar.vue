<template>
    <header class="row align-center">
        <img src="../assets/logo.png" alt="Meevy" id="home-logo" />
        <ul class="nav-links row">
            <a href="#">
                <li class="nav-link">Features</li>
            </a>
            <a href="#">
                <li class="nav-link">Download</li>
            </a>
            <a href="#">
                <li class="nav-link">Support</li>
            </a>
        </ul>
        <button>
            Join Waitlist
        </button>
    </header>
</template>

<script>
export default {
    name: 'navbar'
}
</script>

<style scoped>
#home-logo {
    width: 6em;
    height: 2em;
}

header {
    padding: 1em;
    width: 100%;
    height: 8vh;
    position: fixed;
    top: 0;
}

header ul {
    flex-grow: 1;
    justify-content: center;
}

header a {
    color: inherit;
}

header ul .nav-link {
    padding: 0 1em;
    font-size: small;
}
button{
    background-color: black;
    color: white;
    padding: 0.6em 1.2em
}
</style>