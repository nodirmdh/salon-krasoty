<template>
    <div class="card-item">
        <img :src="img" alt="">
        <div class="item-info">
            <h1>{{title}}</h1>
            <p>{{subtitle}}</p>
            <span class="price">{{price}} &#x20bd;</span>
        </div>
    </div>
</template>

<script>
export default {
    props: {
        title: String,
        img: String,
        subtitle: String,
        price:Number
    },
}
</script>

<style lang="scss" scoped>
    .card-item{
        width: 100%;
        padding: 10px ;
        border: 2px solid rgba(51, 51, 51, 0.349);
        border-radius: 12px;
        margin: 10px 0;
        img{
            height: 200px;
            border-radius: 10px;
        }
    }

    .item-info{
        h1{
            font-size: 20px;
            margin: 10px 0;
            color: #fff;
        }
        p{
            font-size: 18px;
            color: rgb(255, 184, 184);
            max-height: 100px;
            overflow-y: scroll;
        }
    }
    .price{
        display: inline-block;
        font-family: Verdana, Geneva, Tahoma, sans-serif;
        font-size: 25px;
        font-weight: 200;
        margin: 10px 0;
        color: rgb(255, 255, 255);
        border-bottom: 2px solid #fff;
    }
</style>