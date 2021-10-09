<template>
    <section id="hero">
        <div class="row mx-0">
            <div class="col-12 col-md-10 offset-md-1 col-lg-8 offset-lg-2 text-center text-section">
                <h1>Men<span class="text-red">s</span>ch</h1>
                <h2>Maatschappelijk en <wbr>sociale cohesie</h2>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'Hero',
}
</script>

<style scoped>
section {
    background-image: url("~@/assets/images/hero/hero.jpg");
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
    min-height: 100vh;
    background-color: black;
}

h2 {
    color: black;
    text-transform: unset;
    margin-bottom: unset;
}

.text-section {
    white-space: nowrap;
    margin-top: 200px;
}
</style>
