<template>
    <section class="banner">
        <div class="container" id="third">
            <div class="text">
                <h1>САМЫЕ УМНЫЕ ПРОЕКТЫ</h1>
                <h3>РЕАЛИЗУЕМ САМЫЕ СМЕЛЫЕ РЕШЕНИЯ В РОССИИ!</h3>
            </div>
            <button>ВАШ ЗАПРОС</button>
        </div>
    </section>
</template>

<script>

</script>

<style>
.banner {
    padding: 50px 0;
    background: #F7654A;
}

#third {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.text>h1 {
    font-weight: 700;
    font-size: 48px;
    color: #fff;
    margin: 0;
}

.text>h3 {
    font-weight: 700;
    font-size: 24px;
    color: #fff;
    margin: 0;
}

button {
    width: 175px;
    height: 49px;
    border: none;
    background-color: #FFF;
    color: #000;
    font-family: 'Oswald', sans-serif;
    font-size: 14px;
    font-weight: 500;
}

button:hover {
    background-color: #dfdfdf;
}

button:active {
    background-color: #bfbfbf;
}

@media screen and (max-width: 1147px) {

    .text>h1 {
        font-size: 35px;
    }

    .text>h3 {
        font-size: 15px;
    }

    #third {
        padding: 0 10vw;
    }
}

@media screen and (max-width: 715px) {
    #third {
        display: grid;
        justify-content: center;
        text-align: center;
        gap: 15px;
    }

    button {
        width: 106px;
        height: 33px;
        font-size: 10px;
        margin: 0 auto;
        display: block;
    }

}

@media screen and (max-width: 500px) {
    .text>h1 {
        font-size: 20px;
    }

    .text>h3 {
        font-size: 10px;
    }
}
</style>