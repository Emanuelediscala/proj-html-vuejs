<script></script>
<template>
    <div class="position-absolute ">
        <h2 class="m-0" >Caring <span>For Life</span></h2>
        <p class="my-4">Kinds Words can be short and easy to speak. but their echoes are truly <br> endless. Avada Health focuses on you as if it was our own family</p>
        <button>LEARN MORE</button>
    </div>
</template>

<style lang="scss" scoped>
@use "../../style/generic.scss" as *;
@use "../../style/variables.scss" as *;

div {
    top: 40% ;
    left: 25%;
}
h2 {
    color: white!important;
    display: inline;
    font-weight: 100!important;
    font-size: 55px;
}
span:last-child {
    color: $primaryColor!important;
}
p{
    color: white;
    white-space: normal;
}
button:hover {
    background-color: white!important;
    color:$primaryColor;
}

</style>