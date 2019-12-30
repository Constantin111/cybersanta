<template>
    <div class="d-flex flex-wrap justify-center content-container-wrap">
        <div class="container container-text">
            <h1><span class="gold">И целого мира мало</span></h1>

            <p class="promo-hello__description">
                Окей, мы уже разобрались с логистикой Санты. Но вот где же будут располагаться его заводы? Наивно думать, что заводы Санты будут пыхтеть в Лапландии. Мы берём пример с лучших и полагаем, что Санта тоже метит в космос. Выбери, где расположить фабрику подарков
            </p>
        </div>

        <div class="santa-accsesuar-wrap">
            <ul class="santa-accses-cont">
                <li class="button-choise santa-golem" name="robot" @mouseover="setTelescopHover()"
                    @mouseout="setTelescopHover()" @click="setTelescopVisible()">Конечно же, в Космическом Центре М.Видео
                </li>
                <li class="button-choise santa-frends" name="scuter" @mouseover="setNiiCenterHover()"
                    @mouseout="setNiiCenterHover()" @click="setNiiCenterVisible()">Научно-Исследовательский Центр тоже подойдет
                </li>
                <li class="button-choise santa-monitor" name="copter" @mouseover="setRaketaHover()"
                    @mouseout="setRaketaHover()" @click="setRaketaVisible()">Договоримся С Илоном Маском и Space X
                </li>
                <li class="button-choise santa-elf" name="sani" @mouseover="setSnegovikHover()"
                    @mouseout="setSnegovikHover()" @click="setSnegovikVisible()">Оставлю в Лапландии — зачем придумывать новое?
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
    export default {
        name: "choise-three",
        props: {
            setTelescopVisible: Function,
            setNiiCenterVisible: Function,
            setRaketaVisible: Function,
            setSnegovikVisible: Function,
            setTelescopHover: Function,
            setNiiCenterHover: Function,
            setRaketaHover: Function,
            setSnegovikHover: Function,
        }
    }
</script>

<style scoped>

</style>