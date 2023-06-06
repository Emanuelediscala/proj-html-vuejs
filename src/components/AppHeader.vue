<script>
import HeadNav from "./HeaderComp/HeadNav.vue"
import HeadCore from "./HeaderComp/HeadCore.vue"
// IMPORTO COMPONENTI
export default {
    components: {
        HeadNav,
        HeadCore
    },
    
    data() {
        return {
            // DEFINISCO ARRAY DI OGGETTI PER NAVBAR 
            linkList: [
                {
                    name: "HOME",
                    id: "#"
                },
                {
                    name: "ABOUT",
                    dropDownList: ["Same Day Appointments",
                        "World Facilities",
                        "Export Doctors",
                        "Complementary Therapies"],
                    id: "#points"
                },
                {
                    name: "DEPARTMENTS",
                    dropDownList: [
                        "General Practise",
                        "Cardiology",
                        "Pediatrics",
                        "Diabetes Care",
                        "Pre-natal Care",
                        "Ultrasound Echocardiogram"],
                    id: "#MedicalDep"
                },
                {
                    name: "ARTICLES",
                    dropDownList: [
                        "Johnsnow",
                        "Tony Stark",
                        "Anna Smith"],
                    id: "#Ourdoctors"
                },
                { 
                    name: "MAKE APPOINTMENT",
                    dropDownList: ["Make your Appointment"],
                    id: "#Form"
                } 
                ]
                }
        }
    }

</script>
<template>
    <!-- PASSO LE PROPS AI COMPONENTI -->
    <header class="position-relative">
        <HeadNav :links="linkList" />
        <HeadCore />
    </header>
</template>
<!-- PARTE LAYOUT CSS -->
<style scoped>
header {
    background-image: url("../assets/img/header-image-homepage.jpg");
    height: 740px;
    background-size: cover;
    background-repeat: no-repeat;
}
</style>
