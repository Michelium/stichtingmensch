<template>
    <section id="goals">
        <div class="row mx-0">
            <div class="col-12 col-md-5 text-center text-md-start">
                <img class="w-100 photo mx-auto" src="~@/assets/images/work/work.jpg" alt="Hoe werken wij">
            </div>
            <div class="col-12 col-md-7">
                <div class="row align-items-center h-100">
                    <div class="col-12 mx-auto">
                        <div class="mt-5 mt-md-0">
                            <h3>Hoe werken wij?</h3>
                            <p>
                                Lorem ipsum dolor sit amet. Eos nesciunt voluptas in quae quam vel placeat dolor et temporibus nisi ut cupiditate sint eos consequuntur repudiandae. Nam voluptatem dolor a magni molestiae ut doloremque neque. Ut voluptas illo At
                                illo accusamus et earum magni et illum soluta aut nobis obcaecati. Et tempore eius aut aliquid commodi est repellendus expedita vel incidunt sunt. <br><br>
                                Et galisum velit cum officia dignissimos est quia maiores. Et architecto quod ea recusandae quam ab ducimus voluptatem qui inventore quae id dolor autem. <br><br>
                                Ut galisum sunt dolore odit eum enim omnis id rerum similique. Ea dolorem minima vel assumenda maiores eum atque voluptatum sit vero delectus. Et amet possimus sed inventore molestiae vel nesciunt distinctio sit reprehenderit vero
                                At dignissimos error et fuga alias?
                            </p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'Work',
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
