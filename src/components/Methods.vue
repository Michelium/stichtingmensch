<template>
    <section id="methods">
        <div class="row mx-0">
            <div class="col-12 col-md-10 offset-md-1 col-lg-8 offset-lg-2">
                <h3>Onze werkwijze</h3>
            </div>
            <div class="col-12 col-md-10 offset-md-1 col-lg-8 offset-lg-2">
                <div class="row">
                    <div class="col-12 col-lg-4 mb-4">
                        <div class="card">
                            <img src="~@/assets/images/methods/method1.png" alt="Methode 1">
                            <hr>
                            <h4 class="text-center fst-italic">Lorem ipsum dolor sit eos</h4>
                            <p class="text-center fst-italic">Lorem ipsum dolor sit amet. Eos nesciunt voluptas in quae quam vel placeat dolor et temporibus</p>
                        </div>
                    </div>
                    <div class="col-12 col-lg-4 mb-4">
                        <div class="card">
                            <img src="~@/assets/images/methods/method1.png" alt="Methode 2">
                            <hr>
                            <h4 class="text-center fst-italic">Lorem ipsum dolor sit eos</h4>
                            <p class="text-center fst-italic">Lorem ipsum dolor sit amet. Eos nesciunt voluptas in quae quam vel placeat dolor et temporibus</p>
                        </div>
                    </div>
                    <div class="col-12 col-lg-4 mb-4">
                        <div class="card">
                            <img src="~@/assets/images/methods/method1.png" alt="Methode 3">
                            <hr>
                            <h4 class="text-center fst-italic">Lorem ipsum dolor sit eos</h4>
                            <p class="text-center fst-italic">Lorem ipsum dolor sit amet. Eos nesciunt voluptas in quae quam vel placeat dolor et temporibus</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'Methods',
}
</script>

<style scoped>
.row {
    background-color: var(--light-green);
    padding: 50px 0;
}

.card {
    padding: 40px 30px;
    -webkit-box-shadow: 0px 0px 10px 0px rgba(0,0,0,0.29);
    -moz-box-shadow: 0px 0px 10px 0px rgba(0,0,0,0.29);
    box-shadow: 0px 0px 10px 0px rgba(0,0,0,0.29);
    transition: 0.2s;
}
.card:hover {
    background-color: #f1f1f1;
}
.card img {
    width: 95%;
    margin: 0 auto 20px auto;
}
.card hr {
    background-color: var(--green);
    border-top: 8px solid var(--green);
    opacity: 1;
    margin-bottom: 30px;
}

@media (min-width: 991px) {
    h4 {
        font-size: 25px;
    }
    p {
        font-size: 20px;
    }
}
</style>
