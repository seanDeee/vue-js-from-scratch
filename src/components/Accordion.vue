<template>
    <section class="accordion">
        <div class="accordion-container">
            <h1> {{ item.title }} </h1>
            <p class="button-trigger" @click="toggle = ! toggle"> Details </p>
            <p class="accordion-description" v-if="toggle"> {{ item.description }} </p>
        </div>
    </section>
</template>

<script>
    export default {
        name: "Accordion",

        props: ['item'],

        data: function() {
            return {
                toggle: false,
            }
        }
    }
</script>

<style scoped>

</style>
