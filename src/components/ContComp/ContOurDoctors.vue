<script>
export default {
    props: {
        doctors:Object
    }
}
</script>
<template>
    <div id="jumbo">
        <div class="container p-2 ">
            <div class="text-center w-50 p-1 mt-4 m-auto">
                <img src="../../assets/img/icon-5.png" class="img-fluid " alt="">
                <h3>MEET OUR DOCTORS</h3>
                <hr class="w-25 m-auto my-4">
                <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Vitae magni dolorem sed ex suscipit dolore
                    rerum provident aperiam. Lorem ipsum dolor, sit amet consectetur adipisicing elit. Fugit assumenda
                    facilis beatae, vero aliquam aut soluta corporis qui omnis.</p>
            </div>
            <div class="my-3 p-2 row gap-3">
                <div v-for="doctor in doctors" class="card p-0">
                    <img :src="doctor.portraitPath" class="card-img-top " alt="">
                    <div class="card-body">
                        <h5 class="card-title"></h5>
                        <p class="card-text"></p>
                        <a href="#" class="btn btn-primary">Go somewhere</a>  
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use "../../style/generic.scss" as *;

#jumbo {
    background-color: #e5e5e5;
}

h3 {
    margin: 10px 0
}
hr {
    border: 1px solid gray;
}
.card {
    width: calc(100% / 3 - 1rem);
}</style>