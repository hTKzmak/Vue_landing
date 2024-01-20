<template>
    <div class="numberBlock" v-for="info in data">
        <h1>{{ info.years }}</h1>
        <h2>ЛЕТ</h2>
        <p>{{ info.description }}</p>
    </div>
</template>

<script>

export default {
    data() {
        return {
            data: [
                { id: 1, years: 26, description: 'на рынке' },
                { id: 2, years: 20, description: 'заботимся об экологии' },
                { id: 3, years: 15, description: 'преподаем технологии' },
                { id: 4, years: 33, description: 'является лидерами' }
            ]
        }
    }
}

</script>

<style>
.numberBlock {
    width: 190px;
    height: 186px;
}

.numberBlock>h1 {
    color: #F7654A;
    font-size: 72px;
    margin: 0;
}

.numberBlock>h2 {
    color: #000;
    font-size: 36px;
    margin: 0;
}

.numberBlock>p {
    color: #999;
    font-size: 18px;
    margin: 0;
}

@media screen and (max-width: 900px) {

    .numberBlock {
        height: 125px;
    }

    .numberBlock>h1 {
        font-size: 50px;
    }

    .numberBlock>h2 {
        font-size: 20px;
    }

    .numberBlock>p {
        font-size: 13px;
    }
}

@media screen and (max-width: 500px) {
    .numberBlock {
        width: 70px;
        height: 100px;
    }

    .numberBlock>h1 {
        font-size: 30px;
    }

    .numberBlock>h2 {
        font-size: 15px;
    }

    .numberBlock>p {
        font-size: 10px;
    }
}
</style>