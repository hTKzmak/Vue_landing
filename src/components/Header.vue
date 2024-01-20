<template>
    <header class="bgFirst">
        <div class="container" id="first">
            <h1>РЕАЛИЗУЕМ КРУПНЕЙШИЕ <br> ПРОЕКТЫ В РОССИИ</h1>
            <h3>стадионы, газопроводы, мосты, дамбы</h3>
            <div class="yearsList">
                <YearsItem></YearsItem>
            </div>
        </div>
    </header>
</template>

<script>

import YearsItem from './YearsItem.vue'

export default {
    components: {
        YearsItem,
    }
}
</script>

<style>
.bgFirst {
    background-image: url(/src/assets/Background.png);
    background-blend-mode: multiply;
    background-repeat: no-repeat;
    background-position: center center;
    background-size: cover;
}

header {
    padding-top: 100px;
    text-align: center;
    display: grid;
    justify-content: center;
}

#first>h1 {
    color: #FFF;
    font-size: 64px;
    margin: 0;
}

#first>h3 {
    color: #FFF;
    font-size: 18px;
}

.yearsList {
    background-color: #fff;
    display: flex;
    justify-content: center;
    gap: 30px;
    width: 1102px;
    height: 300px;
    align-items: center;
}

@media screen and (max-width: 1147px) {
    .yearsList {
        width: 85vw;
        height: 238px;
        gap: 10px;
    }
}

@media screen and (max-width: 900px) {

    .yearsList {
        height: 180px;
    }

    #first>h1 {
        font-size: 45px
    }

    #first>h3 {
        font-size: 15px
    }
}

@media screen and (max-width: 700px) {
    #first>h1 {
        font-size: 30px
    }

    #first>h3 {
        font-size: 13px
    }

    .yearsList {
        width: 460px;
    }
}

@media screen and (max-width: 500px) {
    .yearsList {
        width: auto;
        height: 150px;
    }
}
</style>
