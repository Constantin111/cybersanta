<template>
    <section class="promo d-flex justify-center flex-wrap align-items-center promo-hello">
        <div class="container promo-container">
            <h1 class="promo-hello__title">
                Предновогодний период - всегда
                <br />
                прекрасное время, но очень
                <br />
                напряженное.
            </h1>
            <p class="promo-hello__description">
                В преддверии 2020 года Санте тоже не помешает небольшая порция чудес и
                помощь от каждого из нас. Поэтому мы решили собрать киберотряд. Хорошие
                новости - ты можешь гордо пополнить  его ряды!
            </p>
            <button type="button" @click="$emit('start-begin')" class="btn">
                Продолжить
            </button>
        </div>
    </section>
</template>

<script>
    export default {
        name: "section-hello"
    }
</script>

<style scoped>

</style>