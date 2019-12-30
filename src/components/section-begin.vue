<template>
    <section class="promo d-flex justify-center flex-wrap align-items-center promo-hello">
        <div class="container">
            <h1 class="promo-hello__title">
                Задача отряда особая: нам предстоит
                <br />
                совершить апгрейд Санты
            </h1>
            <p class="promo-hello__description">
                Модернизировав отважную команду эльфов, повозку из оленей, сани, средства связи и фабрику по производству и сбору подарков! Самые передовые технологии из наших магазинов - в твоих руках. Задача любопытная, посмотрим, как ты справишься?
            </p>
            <button type="button" @click="$emit('start-construct')" class="btn">
                Поехали
            </button>
        </div>
    </section>
</template>

<script>
    export default {
        name: "section-begin"
    }
</script>

<style scoped>

</style>