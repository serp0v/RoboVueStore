           v-if="showRobots()"
<template>
    <main class="main-wrapper">
        <div class="main-container">
            <div class="company-name">RoboVue</div>
            <div class="company-description">The largest online store of robots<br>in the world.</div>
           <div
            class="robots"></div>
        </div>
    </main>
</template>

<script>
// import RoboHeader from "./RoboHeader.vue";
// export default {
//     data(){
//         return {

//         }
//     },
//     components: {
//         RoboHeader
//     },
//     methods: {
//         emitrobots() {
//             this.$emit.RoboHeader.showRobots()
//         }
//     }
// }
</script>

<style>
    .main-wrapper {
        height: calc(100% - 188px);
        width: 100%;
        display: flex;
    }
    .main-container {
        height: 100%;
        width: 100%;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        text-align: center;
    }
    .company-name {
        font-size: 96px;
    }
    .company-description {
        font-size: 48px;
        margin-top: -27px;
        padding-bottom: 13px;
    }
    .robots {
        background-color: rgb(212, 12, 12);
        height: 100px;
        width: 100px;
        display: none;
        position: absolute;
        z-index: 9999;
    }
/*  */
    @media(max-width: 768px) {
        .company-name {
            font-size: 80px;
        }
        .company-description {
            font-size: 40px;
            margin-top: -22.5px;
            padding-bottom: 13px;
        }
    }
    @media(max-width: 568px) {
        .company-name {
            font-size: 64px;
        }
        .company-description {
            font-size: 32px;
            margin-top: -18px;
            padding-bottom: 10.4px;
        }
    }
    @media(max-width: 442px) {
        .company-name {
            font-size: 48px;
        }
        .company-description {
            font-size: 24px;
            margin-top: -13.5px;
            padding-bottom: 8px;
        }
    }
</style>