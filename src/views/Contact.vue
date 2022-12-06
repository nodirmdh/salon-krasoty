<template>
    <app-header title="Контакты" back="true"></app-header>
    <div class="card">
        <div class="item">
            <img src="../assets/Compass-1.svg" alt="">
            <h1>Россия, Москва, ул.Большой Кузьмечь, улица 1</h1>
        </div>
        <br>    
        <div class="info">
            <img src="../assets/Shop-1.svg" alt="">
            <div class="info-flex">
                <p>Режим работы:</p>
                <span>пн-пт с 9.00 до 18.00</span>
                <span>Перерыв:с 13.00 до 14.00</span>
                <span>Выходные: Сб / Вс</span>

            </div>
        </div>
        <div class="group">
            <div class="item">
                <img src="../assets/Phone-1.svg" alt="">
                <a href="">+998 99 700 27 44</a>
            </div>
            <div class="item">
                <img src="../assets/Phone-1.svg" alt="">
                <a href="">+998 93 102 27 44</a>
            </div>
        </div>
            <div class="item">
                <img src="../assets/Message-1.svg" alt="">
            <a href="">makhmudovnodir111@gmail.com</a>
        </div>
        <div class="group">
            <div class="item">
                <img src="../assets/insta-1.svg" alt="">
                <a href="">instagram</a>
            </div>
            <div class="item">
                <img src="../assets/Phone-1.svg" alt="">
                <a href="">whatsapp</a>
            </div>

        </div>
        
        <div style="position:relative;"><a href="https://yandex.uz/maps/213/moscow/?utm_medium=mapframe&utm_source=maps"
                style="color:#eee;font-size:12px;position:absolute;top:0px;">Москва</a><a
                href="https://yandex.uz/maps/213/moscow/?l=sat%2Cskl%2Ctrf%2Ctrfe&ll=37.584522%2C55.747384&utm_medium=mapframe&utm_source=maps&z=20"
                style="color:#eee;font-size:12px;position:absolute;top:14px;">Яндекс Карты</a><iframe
                src="https://yandex.uz/map-widget/v1/-/CCUjJHfLDD" width="535" height="400" frameborder="1" background="#333"
                allowfullscreen="true" style="position:relative;"></iframe></div>
        <div style="position:relative;"><a href="https://yandex.uz/maps/213/moscow/?utm_medium=mapframe&utm_source=maps"
                style="color:#eee;font-size:12px;position:absolute;top:0px;">Москва</a><a
                href="https://yandex.uz/maps/213/moscow/?l=sat%2Cskl%2Ctrf%2Ctrfe&ll=37.584522%2C55.747384&panorama%5Bdirection%5D=53.832758%2C-4.979778&panorama%5Bfull%5D=true&panorama%5Bpoint%5D=37.584160%2C55.747281&panorama%5Bspan%5D=121.906860%2C60.000000&utm_medium=mapframe&utm_source=maps&z=20"
                style="color:#eee;font-size:12px;position:absolute;top:14px;">Яндекс Карты</a><iframe
                src="https://yandex.uz/map-widget/v1/-/CCUjJHbOdA" width="535" height="400" frameborder="1"
                allowfullscreen="true" style="position:relative;"></iframe></div>
        
    </div>
</template>

<script>
import AppHeader from '@/components/AppHeader.vue';
export default {
    setup() {

    },
    components: { AppHeader }
}
</script>

<style lang="scss" scoped>
h1, a, span, p{
    color: #fff;
}
.card {
    background: rgba(255, 255, 255, 0.048);
    position: relative;
    display: flex;
    flex-wrap: wrap;
}

.group{
    display: flex;
    align-items: center;
    gap: 20px;
    margin: 20px 0;
}
.info{
    display: flex;
    align-items: center;
    gap: 20px;
    margin-bottom: 20px;
    &-flex{
        display: flex;
        flex-wrap: wrap;
    gap: 20px;
    align-items: center;
    }
}
.item{
    display: flex;
    align-items: center;
    gap: 20px;
}
.map-widget-layout-view{
    background: rgb(0, 0, 0);
}
</style>