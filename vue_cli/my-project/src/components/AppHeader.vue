!<template>
    <header>
        <h1>{{ propsdata }}</h1>
        <button v-on:click="sendText">send</button>
    </header>
</template>

<script>
export default {
    props: ['propsdata'],
    methods: {
        sendText: function () {
            this.$emit('renew','text');
        }
    }
}
</script>

<style></style>