<script>
export default {
    props: {
        links: Array
    }
}

</script>


<template>
    <!-- NAV BAR WITH LOGO -->
    <nav class="p-3 d-flex justify-content-between mx-3">
        <div>
            <img id="logo" src="../../assets/img/medical_logo_2x_light.png" alt="">
        </div>
        <div>
            <ul class="nav">
                <li class="nav-item" v-for="link in links">
                    <a  class="nav-link active" href="#" aria-current="page">{{ link }}</a>
                </li>
            </ul>
        </div>
    </nav>
</template>

<style lang="scss" scoped>
#logo {
    width: 200px;
}
a {
    color: white!important;
    font-weight: 400;
}
a:hover {
    color: #3BAFBF!important;
}
ul li:last-child {
    padding: 0px 15px!important;
    background-color: #3BAFBF!important;
    border-radius: 5px;
}
ul li:last-child a:last-child:hover{
    color: white!important;
}     


</style>