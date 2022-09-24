<template>
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
</template>

<script>
</script>

<style>
    .header-wrapper {
        width: 100vw;
        height: 8.703vh;
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
    @media (max-height: 1000px) {
        .header-wrapper {
            height: 94px;
        }
    }
</style>