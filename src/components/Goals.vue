<template>
    <section id="goals">
        <div class="row mx-0">
            <div class="col-12 col-md-7">
                <h3>Wat zijn onze doelen?</h3>
                <div class="row left mt-5">
                    <div class="col-md-3 col-xl-3 d-none d-md-block">
                        <div class="image-border">
                            <img src="~@/assets/images/goals/1.svg" id="1" alt="1">
                        </div>
                    </div>
                    <div class="col-12 col-md-8 col-xl-9">
                        <h4>Maatschappelijk en sociale bijdrage</h4>
                        <p>Lorem ipsum dolor sit amet. Eos nesciunt voluptas in quae quam vel placeat dolor et temporibus nisi ut cupiditate sint eos consequuntur repudiandae.</p>
                    </div>
                </div>
                <div class="row left mt-5">
                    <div class="col-md-3 col-xl-3 d-none d-md-block">
                        <div class="image-border">
                            <img src="~@/assets/images/goals/2.svg" id="2" alt="2">
                        </div>
                    </div>
                    <div class="col-12 col-md-8 col-xl-9">
                        <h4>Leveren aan de leefomgeving</h4>
                        <p>Lorem ipsum dolor sit amet. Eos nesciunt voluptas in quae quam vel placeat dolor et temporibus nisi ut cupiditate sint eos consequuntur repudiandae.</p>
                    </div>
                </div>
                <div class="row left my-5">
                    <div class="col-md-3 col-xl-3 d-none d-md-block">
                        <div class="image-border">
                            <img src="~@/assets/images/goals/3.svg" id="3" alt="3">
                        </div>
                    </div>
                    <div class="col-12 col-md-8 col-xl-9">
                        <h4>Verrichten van alle verdere handelingen</h4>
                        <p>Lorem ipsum dolor sit amet. Eos nesciunt voluptas in quae quam vel placeat dolor et temporibus nisi ut cupiditate sint eos consequuntur repudiandae.</p>
                    </div>
                </div>
            </div>
            <div class="col-12 col-md-5">
                <img class="w-100 photo float-end" src="~@/assets/images/goals/goals.jpg" alt="Doelen">
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


.left {
    flex-wrap: wrap-reverse;
}

.image-border {
    border: 2px solid var(--dark-green);
    border-radius: 50%;
    width: 110px;
    height: 110px;
    display: flex;
    justify-content: center;
    align-items: center;
}

.left img {
    width: 75px;
    height: 75px;
    flex-shrink: 0;
}

@media (min-width: 991px) and (max-width: 1265px) {
    .image-border {
        width: 90px;
        height: 90px;
    }
    .left img {
        width: 55px;
        height: 55px;
    }
}

@media (min-width: 33px) and (max-width: 964px) {
    .image-border {
        width: 75px;
        height: 75px;
    }
    .left img {
        width: 45px;
        height: 45px;
    }
}

.photo {
    max-width: 450px
}
</style>
