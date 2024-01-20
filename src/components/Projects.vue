<template>
    <div class="projectItem" v-for="info in data">
        <img :src=info.image alt="">
        <div class="projectItem_text">
            <h2>{{ info.title }}</h2>
            <p>{{ info.description }}</p>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            data: [
                { id: 1, title: 'Многофункциональное здание', description: 'Мы сделали самую красивую арену в Европе. Это открытие стало для нас прорывной точкой для разивтия на следующие десятилетия.', image: 'https://teletype.in/files/f8/f6/f8f60304-dd5c-4a98-930b-4e1166160f8e.jpeg' },
                { id: 2, title: 'IT Колледж', description: 'Современный колледж на базе западной системе образования. Задача стояла в формировании многофункционального здания для решения всех современных проблем колледжа.', image: 'https://vmrucdn.servicecdn.ru/2021.05/original/60afa87282682c3df243a65c.jpg' },
                { id: 3, title: 'Здание выставки', description: 'Самое красивое здание в комплексе выставки достижений народного хозяйства. Данная архитекутура получила самые высокие награды', image: 'https://vdnh.ru/upload/resize_cache/iblock/b7f/1000_1000_1/b7fcf4db2c6bfdef5f1423a06fdd381d.jpg' }
            ]
        }
    }
}
</script>

<style>
img {
    width: 350px;
    height: 380px;
}

.projectItem {
    width: 350px;
    height: 578px;
}

.projectItem_text::before {
    content: "";
    display: block;
    background: #F7654A;
    width: 55px;
    height: 6px;
}

.projectItem_text {
    padding-top: 30px;
    text-align: start;
}

.projectItem_text>h2 {
    color: #404149;
    font-size: 24px;
}

.projectItem_text>p {
    color: #999;
    font-size: 16px;
}
</style>