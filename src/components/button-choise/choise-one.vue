<template>
    <div class="d-flex flex-wrap justify-center content-container-wrap">
        <div class="container container-text">
            <h1><span class="gold">Главное - упряжка</span></h1>

            <p class="promo-hello__description">
                Сани — классная штука, но давно пора отпустить северных оленей на свободу. Ведь мы можем заменить их
                роботизированной техникой. Скорее выбирай, что поможет Санте в транспортировке подарков!
            </p>
        </div>

        <div class="santa-accsesuar-wrap">
            <ul class="santa-accses-cont">
                <li class="robot-santa button-choise" name="robot" @mouseover="setRobotHover()"
                    @mouseout="setRobotHover()" @click="setRobotVisible()">Прямоходящий робот Atlas или четвероногий робот
                    SpotMini
                </li>
                <li class="scuter-santa button-choise" name="scuter" @mouseover="setScuteerHover()"
                    @mouseout="setScuteerHover()" @click="setScuteerVisible()">
                    Скоростной гироскутер
                </li>
                <li class="copter-santa button-choise" name="copter" @mouseover="setDronHover()"
                    @mouseout="setDronHover()" @click="setDronVisible()">Не знающие усталости санта-дроны
                </li>
                <li class="sani-santa button-choise" name="sani" @mouseover="setSaniHover()"
                    @mouseout="setSaniHover()"  @click="setSaniVisible()">Оставлю его в классической упряжке с оленями
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
    export default {
        name: "choise-one",
        props: {
            setRobotVisible: Function,
            setScuteerVisible: Function,
            setDronVisible: Function,
            setSaniVisible: Function,
            setRobotHover: Function,
            setScuteerHover: Function,
            setDronHover: Function,
            setSaniHover: Function,
        }
    }
</script>

<style scoped>

</style>