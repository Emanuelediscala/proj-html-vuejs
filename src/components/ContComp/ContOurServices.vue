<script>
export default {
    props: {
        services: Object
    }
}
</script>
<template>
    <div class="container p-5">
        <div class="m-auto w-50 text-center p-1 mt-4">
            <img src="../../assets/img/icon-6.png" alt="">
            <h3 class="my-1">OUR HEALTH SERVICES</h3>
            <hr class="w-25 m-auto my-4">
            <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quaerat id ea harum, rem beatae modi recusandae
                reiciendis nesciunt. Lorem ipsum, dolor sit amet consectetur adipisicing elit. Officiis similique.</p>
        </div>
        <div id="ServicesPost" class="row m-auto w-100 text-center">
                <div id="card" class="p-1"  v-for="service in services">
                    <img :src="service.iconPath" alt="">
                    <h5>{{service.title}}</h5>
                    <p>{{ service.description }}</p>
                </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use "../../style/generic.scss" as *;

#card {
    width: calc(100% / 3);
}
h5 {
    font-weight: 300;
    margin: 15px 0;
}
#card:hover  h5 {
    color: #3BAFBF;
    cursor: pointer;
}
p {
    font-weight: 200;
    color: gray;
}
</style>