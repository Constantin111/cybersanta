<template>
    <div class="d-flex flex-wrap justify-center content-container-wrap">
        <div class="container container-text">
            <h1><span class="gold">Санта 🎅 connecting people?</span></h1>

            <p class="promo-hello__description">
                Орбитальные заводы, заряженные солнечной энергией, — вполне в стиле обновленного Санты. Поздравляем, ты причастен к прорыву: космический Санта однозначно круче старомодного бородача из Северной Европы! Или нет? Настало время подумать над связью для Санты. Что выберешь?
            </p>
        </div>

        <div class="santa-accsesuar-wrap">
            <ul class="santa-accses-cont">
                <li class="button-choise santa-golem" name="robot" @mouseover="setRacijaHover()"
                    @mouseout="setRacijaHover()" @click="setRacijaVisible()">Набор раций вполне сойдёт
                </li>
                <li class="button-choise santa-frends" name="scuter" @mouseover="setPowerBankHover()"
                    @mouseout="setPowerBankHover()" @click="setPowerBankVisible()">Дам ему в помощь смартфоны и power bank, пусть меняет при перезарядке
                </li>
                <li class="button-choise santa-monitor" name="copter" @mouseover="setVrHover()"
                    @mouseout="setVrHover()" @click="setVrVisible()">Обеспечу его VR-шлемом с выходом в онлайн
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
    export default {
        name: "choise-fou",
        props: {
            setRacijaVisible: Function,
            setPowerBankVisible: Function,
            setVrVisible: Function,
            setRacijaHover: Function,
            setPowerBankHover: Function,
            setVrHover: Function,
        }
    }
</script>

<style scoped>

</style>