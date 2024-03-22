<script lang="ts">
import NavBar from "./NavBar.vue"
import LogoComponents from "./LogoComponent.vue"

export default {
    name: "HeadScreen",
    components: {
        NavBar,
        LogoComponents
    }
}
</script>

<template>
    <div class="HeadScreen">
        <NavBar />
        <LogoComponents />
    </div>
</template>

<style scoped>

.HeadScreen {
    background-color: #ffffff;
    margin: 0;
    width: 100%;
    height: 615px;
}

</style>