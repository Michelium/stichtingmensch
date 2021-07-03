<template>
    <div class="container-fluid p-0">
        <Header/>
        <Hero/>
    </div>
    <div class="row mx-0">
        <div class="col-12 col-md-10 offset-md-1 col-lg-8 offset-lg-2">
            <Goals/>
        </div>
    </div>
</template>

<script>

import Hero from "../components/Hero";
import Header from "../components/Header";
import Goals from "../components/Goals";

export default {
    name: 'Home',
    components: {
        Goals,
        Header,
        Hero,
    }
}
</script>
