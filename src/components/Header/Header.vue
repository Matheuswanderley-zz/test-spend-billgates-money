<template>
<div id="wrapper-head">
    <span class="span-title">{{ title }}</span>
</div>
</template>

<script>
export default {
    props: {
        title: String
    }
};
</script>

<style lang="scss" scoped>
#wrapper-head {
    display: flex;
    width: 100%;
    background-color: #fff;
    margin-top: -3.6em;
    height: 7em;
    flex-direction: row;
}

.span-title {
    font-size: 5vh;
    margin-left: 24vw;
    margin-top: 1.5vw;
    font-weight: bold;
}
</style>
