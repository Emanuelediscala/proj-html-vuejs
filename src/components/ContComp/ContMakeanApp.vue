<script>
import { Swiper, SwiperSlide } from 'swiper/vue';
import { FreeMode, Pagination } from 'swiper';
export default {
    components: {
        Swiper,
        SwiperSlide,
    },
    props: {
        carousels: Array
    },
    setup() {
        return {
            modules: [FreeMode, Pagination],
        };
    }
}
</script>
<template>
    <div class="row m-0">
        <div class="text-white bg-Light text-center widCalcx3 p-5">
            <h3 class="my-3">Emegency Care</h3>
            <img src="../../assets/img/wave-divider.png" alt="">
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Saepe animi, sequi inventore quo officiis eius sunt
            </p>
            <button class="bg-Light">LEARN MORE</button>
        </div>
        <div class="text-white bg-Medium text-center widCalcx3 p-5">
            <h3 class="my-3">Expert Diagnostics</h3>
            <img src="../../assets/img/wave-divider.png" alt="">
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Saepe animi, sequi inventore quo officiis eius sunt
            </p>
            <button class="bg-Medium">LEARN MORE</button>
        </div>
        <div class="text-white bg-Dark text-center widCalcx3 p-5">
            <h3 class="my-3">Superb Rehabilitation</h3>
            <img src="../../assets/img/wave-divider.png" alt="">
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Saepe animi, sequi inventore quo officiis eius sunt
            </p>
            <button class="bg-Dark">LEARN MORE</button>
        </div>
    </div>
    <div id="Form">
        <div class="w-50 m-auto text-center text-white p-5">
            <h2 class="mt-5">Make An Appointment</h2>
            <hr class="text-white w-25 m-auto my-3">
            <p class="fw-light">Lorem ipsum dolor sit amet consectetur, adipisicing elit. Deleniti nobis possimus doloremque
                quis nulla fugit Lorem ipsum dolor sit amet consectetur adipisicing elit. Cumque explicabo molestiae nobis
                magnam optio incidunt omnis pariatur sapiente natus expedita! Quis voluptatum culpa,</p>
            <form action="" class="m-auto row mx-0 gap-2">
                <input type="text" class="form-control my-1" value="Name" aria-describedby="basic-addon1">
                <input type="email" class="form-control my-1" value="Email" aria-describedby="basic-addon1">
                <input type="Number" class="form-control my-1" aria-describedby="basic-addon1" placeholder="Phone Number">
                <input type="text" class="form-control my-1" placeholder="&#128197; Appointment Date"
                    aria-describedby="basic-addon1">
                <textarea  cols="30" rows="10" placeholder="How can we help?*">
                </textarea>
                <button id="btnApp" class=" my-2 bg-Medium">MAKE AN APPOINTMENT</button>
            </form>
        </div>
    </div>
    <div id="jumbobgGradient">
        <div class="w-50 m-auto p-3">
            <swiper :slidesPerView="3" :spaceBetween="30" :freeMode="true" 
                :modules="modules" class="mySwiper">
                <swiper-slide v-for="carousel in carousels">
                    <img :src="carousel" alt="">
                </swiper-slide>
            </swiper>
        </div>
    </div>
</template>

<style scoped>
template:first-child {
    background-image: url("../../assets/img/rgb-gradient-bar-for-logo-carrasel.jpg");
}

.bg-Light {
    background-color: #3aafbf;
}

.bg-Medium {
    background-color: #3597c3;
}

.bg-Dark {
    background-color: #327ec7;
}

.widCalcx3 {
    width: calc(100% / 3);
}

h2 {
    font-weight: 300;
}

input {
    background-color: transparent;
    color: gray;
    font-weight: 200;
    border-color: gray;
    width: calc(100% / 2 - 1rem);
}

textarea {
    background-color: transparent;
    color: gray;
    font-weight: 200;
    border-color: gray;
    width: calc(100% - 1.6rem);
}

input::placeholder {
    color: gray;
}

h3 {
    font-weight: 400;
}

button {
    color: white;
    border: 1px solid white;
    padding: 5px 15px;
}
div.bg-Light button:hover {
    background-color: white!important;
    color: #3aafbf!important;
}
div.bg-Medium button:hover {
    background-color: white!important;
    color: #3597c3!important;
}
div.bg-Dark button:hover {
    background-color: white!important;
    color: #327ec7!important;
}
#btnApp {
    width: calc(100% - 1.5rem);
    border: none;
}
#btnApp:hover {
    background-color: white;
    color: #3597c3;
}

#Form {
    background-image: url("../../assets/img/make-an-appointment.jpg");
    height: 740px;
    background-position: center;
}

#jumbobgGradient {
    background-image: url("../../assets/img/rgb-gradient-bar-for-logo-carrasel.jpg");
}
</style>