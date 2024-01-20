<template>
    <footer>
        <div class="container" id="fourth">
            <p>© 2019 Строительная компания</p>
            <p>Разработано лучшей студей</p>
        </div>
    </footer>
</template>

<script>

</script>

<style>
footer {
    font-family: 'Open Sans', sans-serif;
    font-size: 16px;
    color: rgba(255, 255, 255, 1);
    background-color: rgba(64, 65, 73, 1);

}

#fourth {
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 82px;
}

@media screen and (max-width: 1147px) {
    #fourth {
        padding: 0 10vw;
    }
}

@media screen and (max-width: 715px) {
    #fourth {
        display: grid;
        justify-content: center;
        text-align: center;
        padding: 10px 0px;
        gap: 10px;
        height: auto;
    }
}

@media screen and (max-width: 500px) {

    #fourth {
        display: grid;
        justify-content: center;
        text-align: center;
    }

    p {
        font-size: 10px;
    }
}
</style>