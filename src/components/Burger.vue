<template>
    <div class="burger">
        <div class="burger-bars"></div>
    </div>
</template>

<script>
export default {

}
</script>

<style lang="scss">
.burger {
    display: flex;
    align-items: flex-end;
    margin-right: 12px;
}
.burger-bars {
    width: 28px;
    height: 20px;
    position: relative;
    &::before {
        position: absolute;
        content: '';
        width: 28px;
        border-bottom: 3px solid #18216D;
        top: 3px;
    }
    &::after {
        position: absolute;
        content: '';
        width: 20px;
        border-bottom: 3px solid #18216D;
        top: 13px;
        right: 0;
    }
}
</style>