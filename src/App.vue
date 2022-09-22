<template>
    <div class="wrapper">

        <header class="header-wrapper">
            <div class="header-container">
                <div class="logo"><p>RoboVue</p></div>
                <ul class="spa-navigation">
                    <li class="nav-item">Home</li>
                    <li class="nav-item">Robots</li>
                    <li class="nav-item">Software</li>
                    <li class="nav-item">Contact</li>
                </ul>
                <div class="log-sign">
                    <button class="log-in">
                        <p>Log in</p>
                    </button>
                    <button class="sign-up">
                        <p>Sign up</p>
                    </button>
                </div>
            </div>
            <div class="header-container-mobile">
                <div class="logo"><p>RoboVue</p></div>
                <div class="burger-menu">
                    <svg width="33" height="25" viewBox="0 0 33 25" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <line y1="0.522476" x2="33" y2="0.522476" stroke="white"/>
                        <line y1="12.1404" x2="33" y2="12.1404" stroke="white"/>
                        <line y1="23.7584" x2="33" y2="23.7584" stroke="white"/>
                    </svg>
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
    /* header-wrapper */
    
    .header-wrapper {
        width: 100%;
        height: 8.703%;
        display: flex;
        justify-content: center;
        align-items: center;
    }
    .header-container {
        max-width: 1102px;
        margin: 0 auto;
        height: 60px;
        display: flex;
        flex-direction: row;
        background-color: rgb(255, 255, 255);

    }
    .logo {
        display: flex;
        align-items: center;
        font-size: 36px;
        border: 1px solid #000;
        padding-left: 7px;
        padding-right: 7px;
        height: 60px;
    }
    .spa-navigation {
        display: flex;
        flex-direction: row;
        align-items: center;
        padding-left: 81px;
        padding-right: 81px;
    }
    .nav-item {
        list-style: none;
        font-size: 36px;
    }
    .nav-item ~ .nav-item {
        margin-left: 57px;
    }
    .log-sign {
        display:flex;
        align-items: center;
        flex-direction: row;
        font-size:36px;
    }
    .log-sign > button {
        display: flex;
        font-size: 36px;
        padding-left: 7px;
        padding-right: 7px;
        height: 58px;
        border: 1px solid #000000;
        justify-content: center;
        align-items: center;
    }
    button > p {
        text-align: center;
        display: flex;
        justify-content: center;
        align-items: center;
    }
    .log-sign > button ~ button {
        margin-left: 43px;
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
        .footer-wrapper {
        }
        .footer-container {
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