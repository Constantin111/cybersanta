<template>
    <div class="d-flex flex-wrap justify-center content-container-wrap">
        <div class="container container-text">
            <h1><span class="gold">Санта-центр создан, что делаем после?</span></h1>

            <p class="promo-hello__description">
                Чтобы отследить, все ли подарки отправлены и нашли своих получателей, Санте понадобятся внушительные инструменты, чем ты его оснастишь?
            </p>
        </div>

        <div class="santa-accsesuar-wrap">
            <ul class="santa-accses-cont">
                <li class="button-choise santa-golem" name="robot" @mouseover="setBinokleHover()"
                    @mouseout="setBinokleHover()" @click="setBinokleVisible()">Биноклем и телескопом
                </li>
                <li class="button-choise santa-frends" name="scuter" @mouseover="setSsdDiscHover()"
                    @mouseout="setSsdDiscHover()" @click="setSsdDiscVisible()">Мощным SSD, чтобы компьютер работал с данными гораздо быстрее
                </li>
                <li class="button-choise santa-monitor" name="copter" @mouseover="setSetiHover()"
                    @mouseout="setSetiHover()" @click="setSetiVisible()">Стабильным 5G интернетом
                </li>
                <li class="button-choise santa-elf" name="sani" @mouseover="setMailBoxHover()"
                    @mouseout="setMailBoxHover()" @click="setMailBoxVisible()">Почта Санты уже так привычна
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
    export default {
        name: "choise-five",
        props: {
            setBinokleVisible: Function,
            setSsdDiscVisible: Function,
            setSetiVisible: Function,
            setMailBoxVisible: Function,
            setBinokleHover: Function,
            setSsdDiscHover: Function,
            setSetiHover: Function,
            setMailBoxHover: Function,
        }
    }
</script>

<style scoped>

</style>