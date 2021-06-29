<template>
    <div class="container-fluid p-0">
        <Hero/>
    </div>
    <div class="row mx-0">
        <div class="col-12 col-md-10 offset-md-1 col-lg-8 offset-lg-2">

        </div>
    </div>
</template>

<script>

import Hero from "../components/Hero";

export default {
    name: 'Home',
    components: {
        Hero,
    }
}
</script>
