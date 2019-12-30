<template>
    <div class="d-flex flex-wrap justify-center content-container-wrap">
        <div class="container container-text">
            <h1><span class="gold">Сделал дело - вознагради себя смело!</span></h1>

            <p class="promo-hello__description">
                Ура, миссия завершилась, подарки доставлены, мир уже закружился в новогоднем праздновании. Санта может отдохнуть. А теперь выбери, как ему расслабиться после сложного рабочего дня?
            </p>
        </div>

        <div class="santa-accsesuar-wrap">
            <ul class="santa-accses-cont">
                <li class="button-choise santa-golem" name="robot" @mouseover="setCapCoffeHover()"
                    @mouseout="setCapCoffeHover()" @click="setCapCoffeVisible()">Приготовить вкусный кофе
                </li>
                <li class="button-choise santa-frends" name="scuter" @mouseover="setGlassJuceHover()"
                    @mouseout="setGlassJuceHover()" @click="setGlassJuceVisible()">Свежевыжатый сок, чтобы восполнить силы
                </li>
                <li class="button-choise santa-monitor" name="copter" @mouseover="setRetritHover()"
                    @mouseout="setRetritHover()" @click="setRetritVisible()">Устроить себе виртуальный Санта-ретрит где-нибудь в горах Тибета
                </li>
                <li class="button-choise santa-elf" name="sani" @mouseover="setPieCakeHover()"
                    @mouseout="setPieCakeHover()" @click="setPieCakeVisible()">Оливье и мандарины - лучший набор для празднований ever!
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
    export default {
        name: "choise-six",
        props: {
            setCapCoffeVisible: Function,
            setGlassJuceVisible: Function,
            setRetritVisible: Function,
            setPieCakeVisible: Function,
            setCapCoffeHover: Function,
            setGlassJuceHover: Function,
            setRetritHover: Function,
            setPieCakeHover: Function,
        }
    }
</script>

<style scoped>

</style>