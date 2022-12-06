<template>
    <app-header title="ASAD"  ></app-header>
    <router-link to="/about">
        <div class="card">
            <img src="../assets/user.svg" alt="">
            <div class="card-subtitle">
                <h2>Наш специалист</h2>
            </div>
        </div>
    </router-link>
    <router-link to="/service">
        <div class="card">
            <img src="../assets/item.svg" alt="">
            <div class="card-subtitle">
                <h2>Наши услуги</h2>
            </div>
        </div>
    </router-link>
    <router-link to="/contact">
        <div class="card">
            <img src="../assets/date.svg" alt="">
            <div class="card-subtitle">
                <h2>Контакты</h2>
            </div>
        </div>
    </router-link>
</template>

<script>
import AppHeader from '@/components/AppHeader.vue';

export default {
    setup() {

    },
    components: { AppHeader }
}

</script>
<style lang="scss" >
a {
    text-decoration: none;
    color: #000;
}

.card {
    width: 98%;
    margin: 0 auto;
    display: flex;
    align-items: center;
    padding: 25px;
    background: rgba(255, 255, 255, 0.164);
    border-radius: 10px;
    margin: 10px auto;
    border: 1px solid rgb(0, 0, 0);
    img {
        background-color: rgb(255, 0, 0);
        color: rgb(255, 255, 255);
        padding: 8px;
        border-radius: 50%;
        box-sizing: content-box;
        filter: invert(160%) sepia(0%) saturate(100%) hue-rotate(144deg) brightness(108%) contrast(200%);
    }
    &-subtitle{
        h2{
            padding-left: 14px;
    font-style: normal;
    font-weight: 400;
    font-size: 20px;
    line-height: 24px;
    width: 100%;
    overflow: hidden;
    position: relative;
    color: #fff;
        }
    }
}
</style>