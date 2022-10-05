<template>
    <section id="goals">
        <div class="row mx-0">
            <div class="col-12 col-md-7">
                <h3>Missie en visie</h3>
                <div class="row left mt-0 mt-md-5">
                    <div class="col-12">
                        <p>Maatschappelijke en sociale bijdrage en leveren aan de leefomgeving ter bevordering van de cohesie en ontwikkeling van de mens. <br><br>
                            Het verrichten van alle verdere handelingen, die met het vorenstaande in de ruimste zin verband houden of daartoe bevorderlijk kunnen zijn.</p>
                    </div>
                </div>
            </div>
            <div class="col-12 col-md-5 text-center text-md-start">
                <img class="w-100 photo float-none float-md-end" src="~@/assets/images/goals/goals.jpg" alt="Doelen">
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'Goals',
}
</script>

<style scoped>
@media (min-width: 991px) {
    p {
        font-size: 20px;
    }
}

img {
    border-radius: 10px;
}
.photo {
    max-width: 450px
}
</style>
