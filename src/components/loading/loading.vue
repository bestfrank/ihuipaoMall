<template>
    <div id="loading">
        <img src="../../images/httpLoading.svg">
    </div>
</template>

<script>
export default {
    name: 'loading',
    data(){
        return{
        }
    },
}
</script>

<style lang="scss" scoped>
@import '../../style/common';
@import '../../style/mixin';

#loading {
    width: 100%;
    height: 100%;
    position: fixed;
    top: 0;
    left: 0;
    z-index: 999999999;
    background: rgba(0, 0, 0, .3);
    &.fade-enter {
        opacity: 1
    }
    img {
        position: absolute;
        top: 50%;
        left: 50%;
        width: 5rem;
        transform: translate(-50% ,-50%);
    }
}

</style>
