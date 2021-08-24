<template>
    <header class="header">
        <div class="container">
            <a href="" class="header-logo">
                <img src="../assets/img/logo.svg" alt="meeting-logo" class="header-logo_svg">
            </a>
            <NavMenu v-if="!mobileView"/>
            <Burger v-if="mobileView"/>
        </div>
    </header>

</template>

<script>
import NavMenu from './NavMenu.vue'
import Burger from './Burger.vue'
export default {
    components: {
        NavMenu,
        Burger
    },
    data() {
        return {
            mobileView: false,
            showNav: false
        }
    },
    methods: {
        handleView() {
            this.mobileView = window.innerWidth <= 900;
        }
    },
    created() {
        this.handleView();
    }
}
</script>

<style lang="scss" scoped>
.header {
    position: relative;
}
.container {
    padding: 25px 0;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
}
.header-logo {
    margin-right: 110px;

    @media screen and (max-width: 1100px) {
        margin-right: 60px;
    }
    @media screen and (max-width: 1000px) {
        margin-right: 30px;
    }
    @media screen and (max-width: 600px) {
        height: 20px;
        width: 70px;
    }

    & img {
        @media screen and (max-width: 600px) {
            height: 20px;
            width: 70px;
        }
    }
}
</style>