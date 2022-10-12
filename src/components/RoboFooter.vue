<template>
    <footer class="footer-wrapper">
        <div class="footer-container">
            <p class="licence">Nothing is not protected. Even robots. Beep Boop.</p>
        </div>
    </footer>
</template>

<script>
</script>

<style>
    .footer-wrapper {
        height: 94px;
        width: 100%;
        display: flex;
        justify-content: center;
        align-items: center;
        background-color: rgb(0, 0, 0);
    }
    .footer-container {
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
    /* @media (max-height: 1000px) {
        .footer-wrapper {
            height: 94px;
        }
    } */
        /* @media (max-height: 1000px) {
        .footer-wrapper {
            height: 94px;
        }
    } */
    @media(max-width: 768px) {
        .footer-container {
            font-size: 20px;
        }
    }
    @media(max-width: 568px) {
        .footer-container {
            font-size: 16px;
        }
    }
</style>