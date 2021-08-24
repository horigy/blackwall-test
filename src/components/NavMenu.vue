<template>
    <div class="navigation">
        <div class="navigation-desktop">
            <nav class="nav-menu">
                <a href="" class="nav-item" v-for="(item, index) in links" :key="index">{{item}}</a>
            </nav>
            <div class="nav-right">
               <a href="" class="login">Sign in</a>
                <button class="download">Download</button>
            </div>
        </div>
    </div>
</template>

<script>
import Burger from './Burger.vue'
export default {
    components: {
        Burger
    },
    data() {
        return {
            links: ['Home', 'Feature', 'Pricing', 'Solution', 'Faq'],
        }
    }
}
</script>

<style lang="scss" >
.navigation {
    flex: 1;
    font-weight: 500;
    font-size: 18px;
}
.navigation-desktop {
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-between;
}
.nav-menu {
    width: 507px;
    display: flex;
    justify-content: space-between;
}
.nav-right {
    display: flex;
    align-items: center;
}
.login {
    margin-right: 45px;

    @media screen and (max-width: 1000px) {
        margin-right: 30px;
    }
}
.download {
    padding: 16px 28px;
    color: #fff;
    background-color: #18216D;
    border-radius: 6px;
}
</style>