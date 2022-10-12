<template>
    <div class="wrapper">
        <robo-header />
        <robo-main>
            <!-- <robots-container></robots-container> -->
        </robo-main>
        <robo-footer />
    </div>
</template>

<script>
export default {
    // setup() {
    // },
    components: {
        RoboHeader,
        RoboMain,
        RoboFooter,
        // RobotsContainer,
    }
}
    import RoboHeader from "./components/RoboHeader.vue";

    import RoboMain from "./components/RoboMain.vue";
    // import RobotsContainer from "./components/main_child/RobotsContainer.vue";

    import RoboFooter from "./components/RoboFooter.vue";
</script>

<style>
    @import url('https://fonts.googleapis.com/css2?family=Oswald&display=swap');
    * {
        box-sizing: border-box;
        font-family: 'Oswald', sans-serif;
    }
    body, html {
        margin: 0;
        padding: 0;
        overflow: hidden;
    }
    .wrapper {
        height: 100vh;
        width: 100vw;
        min-width: 320px;
        min-height: 500px;
        display: flex;
        flex-direction: column;
    }
</style>