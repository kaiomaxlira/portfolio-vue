<script lang="ts">
import NavBar from "./NavBar.vue"
import LogoComponent from "./LogoComponent.vue"

export default {
    name: "HeadScreen",
    components: {
        NavBar,
        LogoComponent
    }
}
</script>

<template>
    <div class="HeadScreen">
        <NavBar />
        <LogoComponent />
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