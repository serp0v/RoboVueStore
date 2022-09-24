<template>
    <main class="main-wrapper">
        <div class="main-container">
            <div class="company-name">RoboVue</div>
            <div class="company-description">The largest online store of robots<br>in the world.</div>
        </div>
    </main>
</template>

<script>
</script>

<style>
    .main-wrapper {
        height: 82.5925vh;
        width: 100vw;
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
/*  */
    @media(max-width: 700px) {
        .company-name {
            font-size: 14vw;
        }
        .company-description {
            font-size: 7vw;
            margin-top: -4vw;
        }
    }
    @media (max-height: 700px) {
        .company-name {
            font-size: 14vh;
        }
        .company-description {
            font-size: 7vh;
            margin-top: -4vh;
        }
    }
    @media (max-height: 1000px) {
        .main-wrapper {
            height: calc(100vh - 188px);
        }
    }
</style>