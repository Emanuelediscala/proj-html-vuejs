<script>
export default {
    props: {
        doctors:Object
    }
}
</script>
<template>
    <div id="jumbo">
        <div class="container p-5 ">
            <div class="text-center w-50 p-1 mt-4 m-auto">
                <img src="../../assets/img/icon-5.png" class="img-fluid " alt="">
                <h3>MEET OUR DOCTORS</h3>
                <hr class="w-25 m-auto my-4">
                <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Vitae magni dolorem sed ex suscipit dolore
                    rerum provident aperiam. Lorem ipsum dolor, sit amet consectetur adipisicing elit. Fugit assumenda
                    facilis beatae, vero aliquam aut soluta corporis qui omnis.</p>
            </div>
            <div class="my-4 p-3 row gap-3">
                <div v-for="doctor in doctors" class="card p-0">
                    <img :src="doctor.portraitPath" class="card-img-top " alt="">
                    <div class="card-body">
                        <h5 class="card-title mt-3">{{ doctor.name }}</h5>
                        <h5 class="card-title">{{ doctor.profession }}</h5>
                        <p class="card-text">{{ doctor.About }}</p>
                        <div class="d-flex gap-2">
                            <i class="fa-brands fa-square-facebook"></i>
                            <i class="fa-brands fa-square-twitter"></i>
                            <i class="fa-brands fa-square-instagram"></i>
                        </div>
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
h5 {
    font-weight: 400;
}
hr {
    border: 1px solid gray;
}
.card {
    width: calc(100% / 3 - 1rem);
}

.fa-brands {
    font-size: 26px
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

</style>