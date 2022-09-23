<template>
    <robo-header />
    <robo-main />
    <robo-footer />

    <div class="wrapper">
        <footer class="footer-wrapper">
            <div class="footer-container">
                <p class="licence">Nothing is not protected. Even robots. Beep Boop.</p>
            </div>
        </footer>
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
    }
}
    import RoboHeader from "./components/RoboHeader.vue";
    import RoboMain from "./components/RoboMain.vue";
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
        display: flex;
        flex-direction: column;
    }
    @media(max-width: 1200px) {
        .header-wrapper {
            background-color: rgb(0, 0, 0);
        }
        .header-container {
            background-color: rgb(0, 0, 0);
            display: none;
        }
        .header-container-mobile {
            display: flex;
        }
        .logo {
            border: none;
            color: white;
        }
    }
    @media(max-width: 580px) {
        .company-name {
            font-size: 64px;
        }
        .company-description {
            font-size: 32px;
            margin-top: -18px;
        }
        .footer-container {
            font-size: 16px;
            margin-bottom: -3px;
        }
    }
    @media(max-width: 390px) {
        .company-name {
            font-size: 48px;
        }
        .company-description {
            font-size: 24px;
            margin-top: -12px;
        }
        .footer-container {
            font-size: 12px;
            margin-bottom: -3px;
        }
    }
    @media(max-height: 700px) {
        .burger-menu {
            margin-top: 0;
        }

    }
    @media(max-height: 530px) {
        .logo {
            font-size: 24px;
        }
        .footer-container {
            font-size: 16px;
            margin-bottom: -3px;
        }
        .burger-menu {
            height: 27px;
            width: 21px;
            margin-top: 3px;
        }
    }
    @media(max-height: 420px) {
        .company-name {
            font-size: 48px;
        }
        .company-description {
            font-size: 24px;
            margin-top: -12px;
        }
    }
</style>