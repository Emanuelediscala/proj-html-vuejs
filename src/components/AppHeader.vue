<script>
import HeadNav from "./HeaderComp/HeadNav.vue"
import HeadCore from "./HeaderComp/HeadCore.vue"

export default {
    components: {
        HeadNav,
        HeadCore
    },
    data() {
        return {
            linkList: ["HOME", "ABOUT", "DEPARTMENTS", "ARTICLES", "MAKE APPOINTMENT"]
        }
    }
}
</script>
<template>
    <header class="position-relative">
        <HeadNav :links="linkList" />
        <HeadCore />
    </header>
</template>

<style scoped>
header {
    background-image: url("../assets/img/header-image-homepage.jpg");
    height: 740px;
    background-size: cover;
    background-repeat: no-repeat;
} 
</style>
