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
            
            <ul class="list-unstyled d-flex gap-3">
                <li class="nav-item dropdown text-white" v-for="(link, i) in links">
                    <a class="nav-link " href="#" role="button" data-bs-toggle="dropdown"
                        aria-expanded="false">
                        {{ link.name }}
                    </a>
                    <ul class="dropdown-menu dropdown-menu-end" v-if="link.name !='HOME'">
                        <li v-for="dropdown in link.dropDownList"><a class="dropdown-item text-dark" :href="link.id">{{ dropdown }}</a></li>
                    </ul>
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
    color: white ;
    font-weight: 400;
}

a:hover {
    color: #3BAFBF !important;
}
ul.dropdown-menu a:hover {
    color:white;
}

ul.list-unstyled > li:last-child {
    padding: 0px 10px !important;
    background-color: #3BAFBF !important;
    border-radius: 5px;
}
ul.list-unstyled:hover > li:last-child {
    background-color: white!important;
    color:#3BAFBF!important ;
}



</style>