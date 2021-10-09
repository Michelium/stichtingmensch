<template>
    <section id="contact">
        <div class="row mx-0">
            <div class="col-12 col-md-5 offset-md-1 col-lg-4 offset-lg-2 mb-5 mb-md-0">
                <h3 class="mb-5">Contacteer ons</h3>
                <p>
                    Stichting Mensch <br>
                    Haverschmidtstraat 10 <br>
                    2522 VN Den Haag
                </p>
                <table>
                    <tr>
                        <th><p>E-MAIL:</p></th>
                        <td><p>info@stichtingmensch.nl</p></td>
                    </tr>
                    <tr>
                        <th>&nbsp;</th>
                    </tr>
                    <tr>
                        <th><p>KVK:</p></th>
                        <td><p>60597364</p></td>
                    </tr>
                </table>
            </div>
            <div class="col-12 col-md-5 col-lg-4">
                <form class="mt-4" action="" @submit.prevent="sendEmail">
                    <div v-if="success" class="alert alert-success alert-dismissible fade show" role="alert">
                        <p class="text-dark">Uw bericht is verstuurd! We komen zo spoedig mogelijk bij u terug!</p>
                    </div>
                    <div class="form-group mb-3">
                        <label class="fst-italic" for="name">Volledige naam:</label>
                        <input v-model="name" class="form-control bg-light py-2" type="text" name="name" id="name" autocomplete="off" required>
                    </div>
                    <div class="form-group mb-3">
                        <label class="fst-italic" for="email">E-mailadres:</label>
                        <input v-model="email" class="form-control bg-light py-2" type="email" name="email" id="email" autocomplete="off" required>
                    </div>
                    <div class="form-group mb-3">
                        <label class="fst-italic" for="phone">Telefoonnummer</label>
                        <input v-model="phone" class="form-control bg-light py-2" type="text" name="phone" id="phone" autocomplete="off">
                    </div>
                    <div class="form-group mb-3">
                        <label class="fst-italic" for="message">Bericht:</label>
                        <textarea v-model="message" class="form-control bg-light py-2" name="message" id="message" autocomplete="off" required rows="4"></textarea>
                    </div>
                    <button :disabled="!loaded"  type="submit" class="btn">VERSTUUR</button>
                </form>
            </div>
        </div>
    </section>
</template>

<script>
import emailjs from 'emailjs-com';

export default {
    name: 'Contact',
    data() {
        return {
            form: {
                name: '',
                email: '',
                phone: '',
                message: '',
            },
            errors: {},
            success: false,
            loaded: true,
        }
    },
    methods: {
        sendEmail(e) {
            if (this.loaded) {
                this.loaded = false;
                this.success = false;
                emailjs.sendForm('service_n68sv0h', 'template_1rt5eiv', e.target, 'user_5EsQHMW2uTGVfimVRKRFU')
                    .then((result) => {
                        console.log('SUCCESS!', result.status, result.text);
                        this.name = '';
                        this.email = '';
                        this.phone = '';
                        this.message = '';
                        this.loaded = true;
                        this.success = true;
                    }, (error) => {
                        this.loaded = true;
                        this.success = false;
                        console.log('FAILED...', error);
                    });
            }

        }
    }
}
</script>

<style scoped>
section {
    margin-bottom: unset!important;
}
.row {
    background-color: var(--light-green);
    padding: 50px 0;
}

table p {
    margin-bottom: unset;
}

th {
    font-weight: normal;
    min-width: 120px;
}

label {
    color: var(--text-light);
}

input,textarea {
    border-radius: 10px;
}

button {
    background-color: var(--green);
    color: white;
    padding: 6px 30px;
    border-radius: 10px;
}

@media (min-width: 991px) {
    p {
        font-size: 20px;
    }
}
</style>
