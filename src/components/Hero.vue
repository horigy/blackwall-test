<template>
    <section class="hero-section">
        <div class="container left-container">
            <div class="hero">
                <h1>The best video online meeting software.</h1>
                <p class="hero-desc">
                    Many desktop publishing packages and web page editors now use Lorem Ipsum as their default
                </p>
                <button class="hero-btn">Start for free</button>
                <img src="../assets/img/hero-bg-mobile.png" alt="" class="hero-bg_mobile" v-if="mobileView">
            </div>
        </div>
        <img src="../assets/img/hero-bg.png" alt="" class="hero-bg" v-if="!mobileView">
    </section>
</template>

<script>
export default {
    data() {
        return {
            mobileView: false,
        }
    },
    methods: {
        handleView() {
            this.mobileView = window.innerWidth <= 400;
        }
    },
    created() {
        this.handleView();
    }
}
</script>

<style lang="scss" scoped>
.container {
    padding-top: 118px;

    @media screen and (max-width: 1200px) {
        padding-top: 100px;
    }

    @media screen and (max-width: 1000px) {
        padding-top: 50px;
    }

    @media screen and (max-width: 900px) {
        padding-top: 75px;
    }

    @media screen and (max-width: 700px) {
        padding-top: 16px;
    }
}
.hero {
    max-width: 500px;

    @media screen and (max-width: 900px) {
        max-width: 50%;
    }

    @media screen and (max-width: 700px) {
        max-width: 55%;
    }

    @media screen and (max-width: 600px) {
        max-width: 90%;
        margin: 0 auto;
        display: flex;
        flex-direction: column;
        align-items: center;
        text-align: center;
    }
}
h1 {
    font-size: 48px;
    line-height: 60px;
    font-weight: 600;
    margin-bottom: 18px;
    @media screen and (max-width: 900px) {
        font-size: 28px;
        line-height: 28px;
    }
}
.hero-desc {
    font-size: 17px;
    line-height: 28px;
    margin-bottom: 33px;

    @media screen and (max-width: 900px) {
        font-size: 14px;
        line-height: 20px;
    }

    @media screen and (max-width: 600px) {
        margin-bottom: 30px;
    }
}
.hero-btn {
    padding: 23px 40px;
    background-color: #00ECD0;
    color: #18216D;
    font-size: 17px;
    font-weight: 600;
    display: flex;
    align-items: center;
    justify-content: center;

    @media screen and (max-width: 900px) {
        font-size: 14px;
        line-height: 17px;
        padding: 11px 17px;
        font-weight: 400;
    }

    @media screen and (max-width: 600px) {
        max-width: 120px;
        margin-bottom: 40px;
        padding: 11px 20px;
    }
}
.hero-bg {
    position: absolute;
    top: 6%;
    right: 12.2%;
    z-index: -1;

    @media screen and (max-width: 1400px) {
        right: 6%;
    }

    @media screen and (max-width: 1300px) {
        right: 0;
    }

    @media screen and (max-width: 1200px) {
        width: 600px;
    }

    @media screen and (max-width: 1000px) {
        width: 500px;
    }

    @media screen and (max-width: 900px) {
        width: 60%;
    }
    @media screen and (max-width: 600px) {
        position: unset;
        width: 100%;
        margin-left: -50px;
    }
}

.hero-bg_mobile {
    width: 100%;
    margin: 0 auto;
}
</style>