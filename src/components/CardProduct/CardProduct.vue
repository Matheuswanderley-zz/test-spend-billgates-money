<template>
<div class="wrapper">
    <img :src="image" class="image" />
    <span class="sku">{{sku}}</span>
    <span class="price">{{price}}</span>
    <div class="buttons-container">
        <button type="button" :id="id" class="button sell" @click="callId">Sell</button>
        <input type="text" class="amount" v-model="value" placeholder="0">
        <button type="button" class="button buy">Buy</button>
    </div>
</div>
</template>

<script>
export default {
    data: () => {
        return {
            value: ''
        };
    },
    props: {
        id: Number,
        image: String,
        sku: String,
        price: String,
        initialValue: String
    },
    methods: {
        callId() {
            let price = this.price.slice(1)
            let value = this.value.toString()
            let ammout = price * value
            return ammout

        }
    }

}
</script>

<style lang="scss" scoped>
.wrapper {
    max-width: 100%;
    height: 305px;
    background-color: #fff;
    margin: 0 auto;
    margin-top: 3vh;
    padding: 20px 15px;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-between;
}

.image {
    max-width: 100%;
    height: 150px;
    padding: 5px 0px;
    object-fit: contain;
}

.sku {
    color: #000;
    padding: 3px 0px;
    font-size: 1.375rem;
    font-weight: bold;
}

.price {
    color: rgb(36, 196, 134);
    font-size: 1.25rem;
}

.buttons-container {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
}

.button {
    width: 90px;
    height: 50px;
    border-radius: 3px;
}

.sell {
    background-color: rgb(241, 242, 246);
    width: 75px;
    height: 39px;
    border: none;
    cursor: pointer;
}

.buy {
    background: linear-gradient(rgb(46, 204, 113), rgb(26, 188, 156));
    width: 75px;
    height: 39px;
    border: none;
    cursor: pointer;
}

.amount {
    max-width: 100px;
    height: 50px;
    background-color: #fff;
    margin: 0px 15px;
    height: 35px;
    border: 1px solid rgb(178, 190, 195);
    text-align: center;
}
</style>
