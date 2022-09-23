<template>
    <robo-header />
    <div class="wrapper">
        <main class="main-wrapper">
            <div class="main-container">
                <div class="company-name">RoboVue</div>
                <div class="company-description">The largest online store of robots<br>in the world.</div>
            </div>
        </main>

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
        RoboHeader
    }
}
    import RoboHeader from "./components/RoboHeader.vue";
</script>

<style>
    @import url('https://fonts.googleapis.com/css2?family=Oswald&display=swap');
    * {
        box-sizing: border-box;
        font-family: 'Oswald', sans-serif;
    }
    body, html {
        height: 100vh;
        width: 100vw;
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
    .main-wrapper {
        height: 82.5925vh;
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
    }
    .footer-wrapper {
        height: 8.703vh;
        width: 100%;
        display: flex;
        justify-content: center;
        align-items: center;
        background-color: rgb(0, 0, 0);
    }
    .footer-container {
        /* max-width: 1102px; */
        /* height: 60px; */
        display: flex;
        flex-direction: row;
        justify-content: center;
        align-items: center;
        color: white;
        font-size: 24px;
        margin-bottom: -3px;
    }
    .licence {
        height: 100%;
        justify-content: center;
        align-items: center;
        display: flex;
    }
    /* mobile */
    .header-container-mobile {
        display: none;
        width: 100%;
        height: 100%;
        align-items: center;
        padding: 0 20px;
    }
    .burger-menu {
        display: flex;
        justify-content: center;
        align-items: center;
        margin-top: 6px;
        margin-left: auto;
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