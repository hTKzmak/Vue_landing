<template>
    <section class="paddingSecond">
        <div class="container" id="second">
            <h1 id="projectsTitle">НАШИ САМЫЕ БОЛЬШИЕ ПРОЕКТЫ</h1>
            <div class="projectsList">
                <Projects></Projects>
            </div>
        </div>
    </section>
</template>

<script>
import Projects from './Projects.vue'

export default {
    components: {
        Projects,
    }
}
</script>

<style>
.paddingSecond {
    padding: 200px 0;
    display: grid;
    justify-content: center;
}

#projectsTitle {
    color: #404149;
    font-size: 36px;
    margin-bottom: 60px;
    text-align: center;
}

.projectsList {
    display: flex;
    gap: 30px;
}

@media screen and (max-width: 1131px) {
    .projectsList {
        display: grid;
        grid-template-columns: repeat(2, calc(50% - 12px));
        grid-gap: 30px;
    }
}

@media screen and (max-width: 800px) {
    .projectsList {
        display: grid;
        justify-content: center;
        grid-template-columns: none;
    }
}

@media screen and (max-width: 600px) {
    #projectsTitle{
        font-size: 20px;
    }
}

</style>