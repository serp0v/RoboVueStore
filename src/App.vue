<template>
    <div class="wrapper">
        <div class="container">

            <header class="header-wrapper">
                <div class="header-container">
                    <div class="logo">RoboVue</div>
                    <ul class="spa-navigation">
                        <li class="nav-item">Home</li>
                        <li class="nav-item">Robots</li>
                        <li class="nav-item">Software</li>
                        <li class="nav-item">Contact</li>
                    </ul>
                    <div class="log-sign">
                        <div class="">Log in</div>
                        <div class="">Sign up</div>
                    </div>
                </div>
            </header>

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
    </div>
</template>

<script>
// export default {
//     setup() {
        
//     },
// }
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
    }
    body {
        height: 100vh;
        width: 100vw;
    }
    .wrapper {
        height: 100%;
        width: 100%;
    }
    .container {
        display: flex;
        max-width: 1200px;
        height: 100%;
        flex-direction: column;
        margin: 0 auto;
    }

    /* header-wrapper */
    
    .header-wrapper {
        width: 100%;
        height: 94px;
        display: flex;
        justify-content: center;
        align-items: center;
        background-color: rgb(0, 0, 0);


    }
    .header-container {
        width: 1102px;
        height: 60px;
        display: flex;
        flex-direction: row;
        background-color: rgb(255, 255, 255);

    }
    .logo {
        display: flex;
        align-items: center;
        font-size: 36px;
    }
    .spa-navigation {
        display: flex;
        flex-direction: row;
        align-items: center;
    }
    .nav-item {
        margin-left: 56px;
        list-style: none;
        font-size: 36px;
    }
    .log-sign {
        display:flex;
        align-items: center;
        flex-direction: row;
        font-size:36px;
        margin-left: 40px;
    }
    .main-wrapper {
        height: 892px;
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
        width: 100%;
        height: 94px;
        display: flex;
        justify-content: center;
        align-items: center;
        background-color: rgb(0, 0, 0);
    }
    .footer-container {
        width: 1102px;
        height: 60px;
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
</style>