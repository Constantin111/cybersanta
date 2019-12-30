<template>
    <div class="d-flex flex-wrap justify-center content-container-wrap">
        <div class="container container-text">
            <h1><span class="gold">Спаси эльфов от изнуряющего труда</span></h1>

            <p class="promo-hello__description">
                Не секрет, что в новогодние праздники эльфийский народец трудится в поте лица. Так что же может помочь облегчить их работу? Тебе решать, как проведут предновогодние дни эти милые сказочные персонажи
            </p>
        </div>

        <div class="santa-accsesuar-wrap">
            <ul class="santa-accses-cont">
                <li class="button-choise santa-golem" name="robot" @mouseover="setManipuljatorHover()"
                    @mouseout="setManipuljatorHover()" @click="setManipuljatorVisible()">Выберу промышленного голема, он точно все вывезет
                </li>
                <li class="button-choise santa-frends" name="scuter" @mouseover="setCatIcecreemHover()"
                    @mouseout="setCatIcecreemHover()" @click="setCatIcecreemVisible()">Соберу друзей, поможем Санте
                </li>
                <li class="button-choise santa-monitor" name="copter" @mouseover="setMonitorHover()"
                    @mouseout="setMonitorHover()" @click="setMonitorVisible()">Напишу программу на своём топовом ноутбуке, чтобы заменить работу эльфов автоматизированным конвейером
                </li>
                <li class="button-choise santa-elf" name="sani" @mouseover="setElfHover()"
                    @mouseout="setElfHover()" @click="setElfVisible()">Лучше эльфов с этой задачей никто и ничто не справится
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
    export default {
        name: "choise-tou",
        props: {
            setManipuljatorVisible: Function,
            setCatIcecreemVisible: Function,
            setMonitorVisible: Function,
            setElfVisible: Function,
            setManipuljatorHover: Function,
            setCatIcecreemHover: Function,
            setMonitorHover: Function,
            setElfHover: Function,
        }
    }
</script>

<style scoped>

</style>