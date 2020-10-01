<template>
<div id="box">
    <img src="../../assets/billgates.jpg" alt="Bill gates" class="img-gates" /><br />
    <span class="span-msg">{{msg}}</span>
</div>
</template>

<script>
export default {
    props: {
        msg: String
    }
}
</script>

<style lang="scss" scoped>
#box {
    max-width: 1000px;
    height: 266px;
    background-color: #fff;
    margin: 0 auto;
    margin-top: 3vh;
}

.img-gates {
    width: 125px;
    height: 125px;
    border-radius: 50%;
    margin-top: 5vh;
}

.span-msg {
    font-size: 5vh;
    font-weight: bold;
    color: #000;
}
</style>
