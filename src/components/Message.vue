<template>
    <p class="msg" :class="msgClass" v-if="msg">{{ msg }}</p>
</template>

<script>
    export default {
        name: 'Message',
        // props: {
        //     msg: '',
        //     msgClass: ''
        // }
        props: ['msg', 'msgClass']
    }
</script>

<style scoped>
    .msg {
        max-width: 500px;
        margin: 20px auto;
        padding: 20px;
        text-align: center;
        border: 1px solid #ccc;
        border-radius: 5px;
    } 

    .success {
        color: #155724;
        background-color: #d4edda;
        border-color: #d6e6cb;
    }
</style>