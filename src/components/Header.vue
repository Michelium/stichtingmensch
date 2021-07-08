<template>
    <section id="header">
        <nav class="navbar navbar-expand-lg navbar-light custom_navbar custom-navbar-light mx-0 px-0 pt-2 pb-0 mb-2 mb-sm-5 navbar-fixed-top" id="custom-navbar">
            <div class="container-fluid">
                <button class="navbar-toggler float-end" type="button" data-bs-toggle="collapse" data-bs-target="#navbarTogglerDemo01" aria-controls="navbarTogglerDemo01" aria-expanded="false" aria-label="Toggle navigation">
                    <span class="navbar-toggler-icon"></span>
                </button>
                <a class="navbar-brand d-block d-lg-none" href="">
                    <img src="~@/assets/images/logo.png" alt="Stichting Mensch">
                </a>
                <div class="row navbar-row mt-1">
                    <div class="col-12 col-md-8 offset-md-1 col-lg-2 offset-lg-1 offset-xxl-2 d-none d-lg-block">
                        <a class="navbar-brand" href="">
                            <img src="~@/assets/images/logo.png" alt="Stichting Mensch">
                        </a>
                    </div>
                    <div class="col-12 col-md-12 col-lg-8 col-xxl-6">
                        <div class="collapse navbar-collapse" id="navbarTogglerDemo01">
                            <ul class="navbar-nav ms-auto">
                                <li class="nav-item"><a @click="scrollTo('#goals', -120)" class="nav-link">Onze doelen</a></li>
                                <li class="nav-item"><a @click="scrollTo('#methods', -85)" class="nav-link">Onze werkwijze</a></li>
                                <li class="nav-item"><a @click="scrollTo('#foundation', -150)" class="nav-link">De stichting</a></li>
                                <li class="nav-item"><a @click="scrollTo('#contact')" class="nav-link">Contact</a></li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
        </nav>
    </section>
</template>

<script>
export default {
    name: "Header",
    methods: {
        scrollTo(selector, yOffset = 0) {
            const el = document.querySelector(selector);
            const y = el.getBoundingClientRect().top + window.pageYOffset + yOffset;

            window.scrollTo({top: y, behavior: 'smooth'});
        }
    },
}

window.addEventListener("scroll", (event) => {
    var navbar = document.getElementById('custom-navbar');

    let scroll = document.body.getBoundingClientRect().top;

    if (scroll < 0) {
        navbar.classList.add('scrolled');
    } else if (scroll === 0) {
        navbar.classList.remove('scrolled')
    }
});
</script>

<style scoped>
.scrolled {
    -webkit-box-shadow: 0px 10px 28px -6px rgba(0,0,0,0.63);
    -moz-box-shadow: 0px 10px 28px -6px rgba(0,0,0,0.63);
    box-shadow: 0px 10px 28px -6px rgba(0,0,0,0.63);
}

.row {
    flex-grow: 1;
}

nav {
    height: 85px;
    background: white;
    left: 0;
    right: 0;
    z-index: 15;
    position: fixed;
}

nav .navbar-brand {
    height: 100%;
}

nav .navbar-brand img {
    max-height: 45px;
}

nav .navbar-nav > .nav-item > .nav-link {
    font-size: 17px;
    padding: .9rem 20px;
    letter-spacing: 1px;
    color: var(--green);
    font-weight: 600;
    text-transform: uppercase;
}

nav .navbar-nav > .nav-item > .nav-link:hover {
    color: black;
    cursor: pointer;
}

@media (min-width: 992px) and (max-width: 1400px) {
    nav .navbar-nav > .nav-item > .nav-link {
        padding: .9rem 13px;
        font-size: 15px;
    }
}

@media (max-width: 992px) {
    nav {
        top: 0;
        padding-bottom: 14px !important;
        background-color: white!important;
        height: unset;
    }

    nav .navbar-brand img {
        max-height: 40px;
    }

    .row {
        width: 102% !important;
    }

    .navbar-brand {
        color: white!important;
        padding-left: 18px;
    }

    nav .row:first-of-type {
        background: white;
    }

    nav .navbar-nav {
        padding-bottom: 10px;
    }

    nav .navbar-nav > .nav-item > .nav-link {
        padding: .5em .9em;
        text-align: start;
    }
}

@media (max-width: 766px) {
    .col-12 {
        text-align: center;
    }

    .navbar-nav {
        float: none !important;
        justify-content: center;
    }
}

@media (max-width: 455px) {
    nav .navbar-brand img {
        max-height: 35px;
    }

    a.nav-link {
        padding: .5em .5em;
    }
}
</style>
