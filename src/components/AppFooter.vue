<script></script>
<template>
    <footer>
    <div class="row m-0">
        <div class="p-5 col-4">
            <img src="../../src/assets/img/medical_logo_2x_dark.png" class="img-fluid" alt="">
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Expedita doloremque voluptatum sint placeat vel ex veniam autem ut, incidunt culpa nesciunt iste eligendi totam, rerum dolorem nam saepe nihil enim.</p>
            <hr>
            <h4 class="fw-light">LEARN MORE ABOUT US</h4>
            <i class="fa-brands fa-square-facebook"></i>
            <i class="fa-brands fa-square-twitter"></i>
            <i class="fa-brands fa-square-youtube"></i>
            <i class="fa-brands fa-square-instagram"></i>
        </div>
        <div id="contacts" class="col-4 p-5">
            <h4 class="fw-light">CONTACT INFORMATION</h4>
            <hr>
            <p class="mb-1"><i class="fa-solid fa-location-dot"></i> 121 King Street,London United Kingdom</p>
            <p><i class="fa-solid fa-phone"></i> 1.800.458.556</p>
        </div>
        <div id="MedicalDep" class="col-4 p-5">
            <h4 class="fw-light">MEDICAL DEPARTMENTS</h4>
            <hr>
            <ul class="p-0">
                <li class="my-1"><i class="fa-solid fa-circle-chevron-right"></i> Cardiology</li>
                <li class="my-1"><i class="fa-solid fa-circle-chevron-right"></i> Pediactrics</li>
                <li class="my-1"><i class="fa-solid fa-circle-chevron-right"></i> Diabetes Care</li>
                <li class="my-1"><i class="fa-solid fa-circle-chevron-right"></i> Pre-natel Care</li>
                <li class="my-1"><i class="fa-solid fa-circle-chevron-right"></i> Ultrasound Echicardiogram</li>
            </ul>
            <span><button>VIEW OUR DEPARTMENTS</button></span>
        </div>
    </div>
</footer>
<div id="legal" class="pt-3">
    <span class="ms-5">@Copyright 2021-2020 | Avanada Theme by Theme Fusion | All Rights Reserved</span>
</div>
</template>

<style scoped>
footer {
    height: 400px;
}
img {
    width: 250px;
}
p {
    color: gray;
}
.fa-brands {
    font-size: 26px;
    padding: 5px;
}
.fa-solid {
    color:#3aafbf;
}
.fa-square-facebook {
    color: #3c5998;
}
.fa-square-twitter {
    color: #54acee;
}
.fa-square-instagram {
    color:#3f729b;
}
.fa-square-youtube {
    color:red;
}
hr {
    border: 2px solid gray;
}
#contacts hr {
    border: 2px solid #3f729b;
    width: 25%;
}
#MedicalDep hr {
    border: 2px solid #3f729b;
    width: 25%;
}
ul {
    list-style: none;
}
li {
    font-weight: 300;
}
#legal {
    background-color: #f7f7f7;
}
button{
    padding: 5px 10px;
    background-color: transparent;
    font-weight: 400;
    border:1px solid 
}
button:hover {
    background-color: black;
    color: white;
}

</style>