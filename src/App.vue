<script>
import AppHeader from "./components/AppHeader.vue"
import AppContent from "./components/AppContent.vue"
import AppFooter from "./components/AppFooter.vue"

export default {
    components: {
        AppHeader,
        AppContent,
        AppFooter
    }
}
</script>

<template>
    <AppHeader/>
    <AppContent/>
</template>

<style lang="scss" scoped>
@use "./style/generic.scss"
</style>
