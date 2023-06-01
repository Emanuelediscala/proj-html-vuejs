<script>

export default {
    props: {
        strongPoint:Object
    },
    data() {
        return {
        }
    }
}
</script>
<template>
    <div class="container py-3 my-2">
        <div class="m-auto text-center">
            <h3>Welcome to Avada Health</h3>
            <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit.  expedita sit. <br> Lorem ipsum dolor sit, Quod dolorem itaque aspernatur dignissimos repellat   </p>
            <div class="d-flex">
                <div id="points" v-for="point in strongPoint">
                    <img :src="point.iconPath" alt="">
                    <h5>{{ point.title }}</h5>
                    <p>{{ point.description }}</p>
                </div>
            </div>
        </div>
    </div>
</template>
<style lang="scss" scoped>

h3 {
    font-weight: 300!important;
}
p {
    line-height:2em;
    margin: 20px 0;
    
}
#points:hover h5 {
        color: #3BAFBF;
        cursor: pointer;
}
h5 {
    white-space: nowrap;
    font-weight: 300;
}
</style>