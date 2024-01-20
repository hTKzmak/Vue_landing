<template>
    <header class="bgFirst">
        <div class="container" id="first">
            <h1>РЕАЛИЗУЕМ КРУПНЕЙШИЕ <br> ПРОЕКТЫ В РОССИИ</h1>
            <h3>стадионы, газопроводы, мосты, дамбы</h3>
            <div class="numbersList">
                <Numbers></Numbers>
            </div>
        </div>
    </header>
</template>

<script>

import Numbers from './Numbers.vue'

export default {
    components: {
        Numbers,
    }
}
</script>

<style>
.bgFirst {
    background-image: url(/src/assets/Rectangle.png);
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

.numbersList {
    background-color: #fff;
    display: flex;
    justify-content: center;
    gap: 30px;
    width: 1102px;
    height: 300px;
    align-items: center;
}

@media screen and (max-width: 1147px) {
    .numbersList {
        width: 864px;
        height: 238px;
        gap: 10px;
    }
}

@media screen and (max-width: 900px) {

    .numbersList {
        height: 180px;
    }

    #first>h1 {
        font-size: 45px
    }

    #first>h3 {
        font-size: 15px
    }

    .numbersList {
        width: 667px;
    }
}

@media screen and (max-width: 700px) {
    #first>h1 {
        font-size: 30px
    }

    #first>h3 {
        font-size: 10px
    }

    .numbersList {
        width: 460px;
    }
}

@media screen and (max-width: 500px) {
    .numbersList {
        width: auto;
        height: 150px;
    }
}
</style>