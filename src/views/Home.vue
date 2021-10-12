<template>
    <div class="container-fluid p-0">
        <Header/>
        <Hero/>
    </div>
    <div class="row mx-0">
        <div class="col-12 col-md-10 offset-md-1 p-0 col-lg-8 offset-lg-2">
            <Goals/>
        </div>
    </div>
    <div class="container-fluid p-0">
        <Methods/>
    </div>
    <div class="row mx-0">
        <div class="col-12 col-md-10 offset-md-1 p-0 col-lg-8 offset-lg-2">
            <Foundation/>
        </div>
    </div>
    <div class="container-fluid p-0">
        <Contact/>
    </div>
</template>

<script>

import Hero from "../components/Hero";
import Header from "../components/Header";
import Goals from "../components/Goals";
import Methods from "../components/Methods";
import Contact from "../components/Contact";
import Foundation from "../components/Foundation";

export default {
    name: 'Home',
    components: {
        Foundation,
        Contact,
        Methods,
        Goals,
        Header,
        Hero,
    }
}
</script>
