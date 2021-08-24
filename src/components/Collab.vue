<template>
    <section class="collab">
        <div class="container left-container">
            <div class="collab-top">
                <h2>Collaborate 2M+ startup and international companies ueses since 2018 </h2>
                <div class="collab-eval">
                    <div class="collab-likes">
                        <div class="likes-num">15k</div>
                        <div class="likes-icons">
                            <ul class="likes-list">
                                <li class="likes-item" v-for="index in 5" :key="index">
                                    <Icon :name="`heart`"/>
                                </li>
                            </ul>
                        </div>
                        <div class="likes-comment">Active Downloads</div>
                    </div>
                    <div class="collab-stars">
                        <div class="stars-num">4.9</div>
                        <div class="stars-icons">
                            <ul class="stars-list">
                                <li class="stars-item" v-for="index in 5" :key="index">
                                    <Icon :name="`star`"/>
                                </li>
                            </ul>
                        </div>
                        <div class="stars-comment">2,938 Rating</div>
                    </div>
                </div>
            </div>
            <div class="collab-bottom">
                <ul class="partners-list">
                    <li class="partners-item" v-for="(item, index) in partners" :key="index">
                        <Icon :name="item"/>
                    </li>
                </ul>
            </div>
        </div>
    </section>
</template>

<script>
import Icon from './SvgIcon.vue'
export default {
    components: {
        Icon
    },
    data() {
        return {
            partners: ['airbnb', 'hubspot', 'google', 'microsoft', 'walmart', 'fedex'],
        }
    }
}
</script>

<style lang="scss" scoped>
.container {
    padding-top: 253px;
    flex-direction: column;

    @media screen and (max-width: 1300px) {
        padding-top: 230px;
    }

    @media screen and (max-width: 1200px) {
        padding-top: 150px;
    }

    @media screen and (max-width: 1000px) {
        padding-top: 130px;
    }

    @media screen and (max-width: 700px) {
        padding-top: 75px;
    }

    @media screen and (max-width: 600px) {
        padding-top: 60px;
    }
}
.collab-top {
    width: 100%;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: space-between;
    margin-bottom: 50px;

    @media screen and (max-width: 600px) {
        flex-direction: column;
        align-items: center;
        margin-bottom: 20px;
    }
}
h2 {
    max-width: 500px;
    font-weight: 600;
    font-size: 36px;
    line-height: 50px;

    @media screen and (max-width: 900px) {
        font-size: 20px;
        line-height: 30px;
        max-width: 50%;
    }
    @media screen and (max-width: 600px) {
        max-width: 100%;
        margin-bottom: 20px;
    }
}
.collab-eval {
    display: flex;
    flex-direction: row;
    align-items: center;
    margin-right: 180px;

    @media screen and (max-width: 1200px) {
        margin-right: 60px;
    }
}
.collab-likes {
    margin-right: 93px;

    @media screen and (max-width: 1100px) {
        margin-right: 30px;
    }
}

.collab-likes, .collab-stars {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: flex-start;
}
.likes-num, .stars-num {
    font-weight: 700;
    font-size: 60px;
    line-height: 70px;
    letter-spacing: -1px;
    margin-bottom: 7px;

    @media screen and (max-width: 900px) {
        font-size: 24px;
        line-height: 30px;
        margin-bottom: 0;
    }
}
.stars-num {
    margin-bottom: 2px;

    @media screen and (max-width: 1100px) {
        margin-bottom: 7px;
    }
    @media screen and (max-width: 900px) {
        margin-bottom: 0;
    }
}
.likes-list, .stars-list {
    display: flex;
    flex-direction: row;
    margin-bottom: 10px;

    @media screen and (max-width: 900px) {
        margin-bottom: 0;
    }
}

.stars-item, .likes-item {
    margin-right: 5px;
    &:last-child {
        margin-right: 0;
    }

    @media screen and (max-width: 900px) {
        width: 8px;
        height: 8px;
    }

    & svg {
        @media screen and (max-width: 900px) {
            width: 8px;
            height: 8px;
            margin-top: -10px;
        }
    }
}
.likes-comment, .stars-comment {
    font-size: 16px;
    line-height: 28px;

    @media screen and (max-width: 900px) {
        font-size: 8px;
    }
}
.collab-bottom {
    width: 100%;
    overflow: hidden;
}
.partners-list {
    display: flex;
    flex-direction: row;
    align-items: center;
    padding-left: 30px;

    @media screen and (max-width: 1100px) {
        padding-left: 0;
    }
    @media screen and (max-width: 900px) {
        flex-wrap: nowrap;
        width: 150%;
    }
}
.partners-item {
    margin-right: 79px;

    @media screen and (max-width: 1400px) {
        margin-right: 60px;
    }

    @media screen and (max-width: 1200px) {
        margin-right: 30px;
    }
    @media screen and (max-width: 900px) {
        width: 20%;
        margin-right: 0;
    }

    & svg {
        @media screen and (max-width: 900px) {
            width: 100%;
        }
        @media screen and (max-width: 700px) {
            height: 20px;
        }
    }
}
</style>