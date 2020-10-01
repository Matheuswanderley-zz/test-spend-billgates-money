<template>
<div id="wrapper">
    <span class="span-money">{{money}}</span>
</div>
</template>

<script>
export default {
    props: {
        money: String
    }
}
</script>

<style lang="scss" scoped>
#wrapper {
    background-image: linear-gradient(rgb(46, 204, 113), rgb(26, 188, 156));
    max-width: 1000px;
    height: 78px;
    margin: 0 auto;
    margin-top: 3vh;
    position: sticky;
    top: 0;
}

.span-money {
    color: #fff;
    font-size: 4vh;
    font-weight: bold;
    position: relative;
    top: 2vh;
}
</style>
