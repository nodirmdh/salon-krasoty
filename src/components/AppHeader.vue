<template>
    <div class="header">
        <router-link to="/" class="header-return" v-if="back">Назад</router-link>
        <div class="build">
            <h1>{{title}}
        </h1>
        </div>
        <div class="build">
            <h2>Беломорская ул., 23
        </h2>
        </div>
        
        
        
            <slot></slot>
    </div>
</template>
<script>
export default {
    props: {
        title: String,
        admin: false,
        back: false
    },
    
}
</script>
<style lang="scss" scoped>

.header {
    width: 600px;
    background: rgba(255, 255, 255, 0.116);
    border-radius: 0 0 10px 10px;
    text-align: center;
    padding: 20px 0;
    display: flex;
    flex-direction: column;
    position: relative;
    z-index: 10;
    top: 0;
    border-bottom: 2px solid #333;
    border-left: 2px solid #333;
    border-right: 2px solid #333;
    a {
        text-decoration: none;
        
    }
    &-user{
        position: absolute;
        right: 30px;
        top: 30px;
    }
    h1 {
        font-weight: 500;
        font-size: 17px;
        line-height: 24px;
        color: #fff;
    }

    h2 {
        font-weight: 500;
        font-size: 15px;
        line-height: 20px;
        color: rgb(255, 255, 255);
    }

    &-return{
        border: 3px solid #333;
        padding: 5px 10px;
        position: absolute;
        left: 30px;
        top: 23px;
        border-radius: 14px;
        transition: 0.5s;
        font-weight: 500;
        color: #fff;
    }
    &-return:hover{
            background: rgba(255, 0, 0, 0.315);
        }
}


</style>