<template>
    <section class="specials">
        <div class="container left-container">
            <div class="specials-head">
                <h3>Our Special Features</h3>
                <p class="specials-desc">
                    We are familiar with offline speed dating flow so we designed out online<br>
                    platform considering all the requirements
                </p>
            </div>

            <ul class="specials-list">
                <li class="specials-item">
                    <div class="specials-item_icon">
                        <Icon :name="`pricing`"/>
                    </div>
                    <div class="specials-item_title">Affordable Pricing</div>
                    <p class="specials-item_text">
                        A dictionary of over 200 Latin words,with a handful of model sentence. structures, to generate Lorem Ipsum
                    </p>
                    <a href="" class="specials-item_link">Learn more</a>
                </li>
                <li class="specials-item">
                    <div class="specials-item_icon">
                        <Icon :name="`reliability`"/>
                    </div>
                    <div class="specials-item_title">Seamless Reliability</div>
                    <p class="specials-item_text">
                        A dictionary of over 200 Latin words,with a handful of model sentence. structures, to generate Lorem Ipsum
                    </p>
                    <a href="" class="specials-item_link">Learn more</a>
                </li>
                <li class="specials-item">
                    <div class="specials-item_icon">
                        <Icon :name="`collab`"/>
                    </div>
                    <div class="specials-item_title">Secure Collaboration</div>
                    <p class="specials-item_text">
                        A dictionary of over 200 Latin words,with a handful of model sentence. structures, to generate Lorem Ipsum
                    </p>
                    <a href="" class="specials-item_link">Learn more</a>
                </li>
            </ul>
        </div>

    </section>
</template>

<script>
import Icon from './SvgIcon.vue'
export default {
    components: {
        Icon
    }
}
</script>

<style lang="scss" scoped>
.container {
    flex-direction: column;
    padding-top: 130px;

    @media screen and (max-width: 1000px) {
        padding-top: 100px;
    }
    @media screen and (max-width: 700px) {
        padding-top: 75px;
    }
    @media screen and (max-width: 600px) {
        padding-top: 50px;
    }
}
.specials-head {
    width: 550px;
    margin-left: 24%;
    letter-spacing: -1px;
    text-align: center;
    margin-bottom: 48px;

    @media screen and (max-width: 1000px) {
        width: 100%;
        margin-left: 0;
    }
    @media screen and (max-width: 600px) {
        margin-bottom: 40px;
    }
}
h3 {
    font-weight: 600;
    font-size: 48px;
    line-height: 64px;
    margin-bottom: 13px;

    @media screen and (max-width: 900px) {
        font-size: 24px;
        line-height: 24px;
    }
}
.specials-desc {
    font-size: 16px;
    line-height: 30px;
    letter-spacing: normal;

    @media screen and (max-width: 900px) {
        font-size: 14px;
        line-height: 20px;
    }
}
.specials-list {
    display: flex;
    flex-direction: row;

    @media screen and (max-width: 700px) {
        flex-direction: column;
    }
}
.specials-item {
    margin-right: 80px;
    width: 30%;
    max-width: 320px;

    @media screen and (max-width: 1400px) {
        margin-right: 60px;
    }
    @media screen and (max-width: 1200px) {
        margin-right: 30px;
    }
    @media screen and (max-width: 900px) {
        margin-right: 20px;
    }
    @media screen and (max-width: 700px) {
        width: 100%;
        margin-right: 0;
        max-width: unset;
        margin-bottom: 20px;
    }
}
.specials-item_icon {
    margin-bottom: 28px;

    @media screen and (max-width: 900px) {
        width: 48px;
        height: 48px;
        margin-bottom: 20px;
    }

    & svg {
        @media screen and (max-width: 900px) {
            width: 48px;
            height: 48px;
        }
    }
}
.specials-item_title {
    font-weight: 600;
    font-size: 24px;
    line-height: 30px;
    margin-bottom: 14px;

    @media screen and (max-width: 900px) {
        font-size: 20px;
        line-height: 24px;
        margin-bottom: 12px;
    }
}
.specials-item_text {
    font-size: 16px;
    line-height: 26px;
    margin-bottom: 30px;

    @media screen and (max-width: 900px) {
        font-size: 14px;
        line-height: 24px;
        margin-bottom: 20px;
    }
}
.specials-item_link {
    font-weight: 500;
    font-size: 20px;
    line-height: 16px;
    margin-top: auto;

    @media screen and (max-width: 900px) {
        font-size: 20px;
        line-height: 24px;
    }
}
</style>