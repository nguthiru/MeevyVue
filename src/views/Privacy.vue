<template>
    <skeleton-vue>
        <section id="privacy-section">

            <h1>Our Privacy Policy</h1>
        </section>
       
    </skeleton-vue>
</template>

<script>
    import SkeletonVue from '../components/Skeleton.vue';
    export default {
        name:'privacy-policy',
        components:{
            SkeletonVue
        }

    }
</script>
<style>
section{
    min-height: 100vh;
    padding: 2em 0;
}

</style>