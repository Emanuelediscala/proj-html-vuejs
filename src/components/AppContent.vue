<script>
// IMPORTO COMPONENTI
import ContIntroduction from "./ContComp/ContIntroduction.vue"
import ContOurDoctors from "./ContComp/ContOurDoctors.vue";
import ContOurServices from "./ContComp/ContOurServices.vue"
import ContFacilities from "./ContComp/ContFacilities.vue"
import ContMakeanApp from "./ContComp/ContMakeanApp.vue";
export default {
    components: {
        ContIntroduction,
        ContOurDoctors,
        ContOurServices,
        ContFacilities,
        ContMakeanApp
    },
    // DEFINISCO ARRAY DI OGGETTI 
    data() {
        return {
            strongPointList: [
                {
                    iconPath: "../src/assets/img/icon-1.png",
                    title: "SAME DAY APPOINTMENTS",
                    description: "Lorem ipsum, dolor  elit.Lorem ipsum  dolor sit, Quod dolorem "
                },
                {
                    iconPath: "../src/assets/img/icon-2.png",
                    title: "WORLD FACILITIES",
                    description: "Lorem ipsum, dolor  elit.Lorem ipsum dolor sit, Quod dolorem "
                },
                {
                    iconPath: "../src/assets/img/icon-3.png",
                    title: "EXPORT DOCTORS",
                    description: "Lorem ipsum, dolor elit .Lorem ipsum dolor sit, Quod dolorem "
                },
                {
                    iconPath: "../src/assets/img/icon-4.png",
                    title: "COMPLEMENTARY THERAPIES",
                    description: "Lorem ipsum, dolor elit.Lorem ipsum dolor sit, Quod dolorem "
                }
            ],
            doctorsList: [
                {
                    portraitPath: "../src/assets/img/doctor-1.jpg",
                    name: "John Snow",
                    profession: "Anesthesiologist",
                    About: "Lorem, ipsum dolor sit amet consectetur adipisicing elit. Culpa vel incidunt officia provident distinctio optio minima beatae ut sunt nam quas id ullam ex et fugit, nobis praesentium quia. Reprehenderit."
                },
                {
                    portraitPath: "../src/assets/img/doctor-2.jpg",
                    name: "Tony Stark",
                    profession: "Cardiologist",
                    About: "Lorem, ipsum dolor sit amet consectetur adipisicing elit. Culpa vel incidunt officia provident distinctio optio minima beatae ut sunt nam quas id ullam ex et fugit, nobis praesentium quia. Reprehenderit."
                },
                {
                    portraitPath: "../src/assets/img/doctor-3.jpg",
                    name: "Anna Smith",
                    profession: "Nurse Pratictioner",
                    About: "Lorem, ipsum dolor sit amet consectetur adipisicing elit. Culpa vel incidunt officia provident distinctio optio minima beatae ut sunt nam quas id ullam ex et fugit, nobis praesentium quia. Reprehenderit."
                }
            ],
            servicesList: [
                {
                    iconPath: "../src/assets/img/icon-14.png",
                    title: "REHABILITATION CENTER",
                    description: "Lorem, ipsum dolor sit amet consectetur adipisicing elit. Culpa vel incidunt officia provident distinctio optio minima beatae ut sunt nam quas id ullam ex et fugit, nobis praesentium quia. Reprehenderit."
                },
                {
                    iconPath: "../src/assets/img/icon-15.png",
                    title: "DENTAL IMPLANTS",
                    description: "Lorem, ipsum dolor sit amet consectetur adipisicing elit. Culpa vel incidunt officia provident distinctio optio minima beatae ut sunt nam quas id ullam ex et fugit, nobis praesentium quia. Reprehenderit."
                },
                {
                    iconPath: "../src/assets/img/icon-16.png",
                    title: "MEDICINE RESEARCH",
                    description: "Lorem, ipsum dolor sit amet consectetur adipisicing elit. Culpa vel incidunt officia provident distinctio optio minima beatae ut sunt nam quas id ullam ex et fugit, nobis praesentium quia. Reprehenderit."
                },
                {
                    iconPath: "../src/assets/img/icon-11.png",
                    title: "BLOOD BANK",
                    description: "Lorem, ipsum dolor sit amet consectetur adipisicing elit. Culpa vel incidunt officia provident distinctio optio minima beatae ut sunt nam quas id ullam ex et fugit, nobis praesentium quia. Reprehenderit."
                },
                {
                    iconPath: "../src/assets/img/icon-12.png",
                    title: "PHARMACEUTICAL ADVICE",
                    description: "Lorem, ipsum dolor sit amet consectetur adipisicing elit. Culpa vel incidunt officia provident distinctio optio minima beatae ut sunt nam quas id ullam ex et fugit, nobis praesentium quia. Reprehenderit."
                },
                {
                    iconPath: "../src/assets/img/icon-13.png",
                    title: "MEDICAL COUNCSELING",
                    description: "Lorem, ipsum dolor sit amet consectetur adipisicing elit. Culpa vel incidunt officia provident distinctio optio minima beatae ut sunt nam quas id ullam ex et fugit, nobis praesentium quia. Reprehenderit."
                },
            ],
            CarouselList: [
                "../../src/assets/img/client-logos-1-200x188.png",
                "../../src/assets/img/client-logos-2-200x188.png",
                "../../src/assets/img/client-logos-3-200x188.png",
                "../../src/assets/img/client-logos-4-200x188.png",
            ]
        }
    }
}
</script>
<template>
    <!-- PASSO LE PROPS AI FIGLI -->
    <main>
        <ContIntroduction :strongPoint="strongPointList" />
        <ContOurDoctors :doctors="doctorsList" />
        <ContOurServices :services="servicesList" />
        <ContFacilities />
        <ContMakeanApp :carousels="CarouselList" />
    </main>
</template>

