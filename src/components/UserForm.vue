
<template>
    <div>
        <Message :msg="msg" :msgClass="msgClass"/>
        <form action="" id="user-form"></form>
        <div class="input-container">
            <label for="name">Name:</label>
            <input type="text" name="name" id="name" v-model="name" placeholder="Digite o seu nome">
        </div>
        <div class="input-container">
            <label for="email">E-mail:</label>
            <input type="text" name="email" id="email" v-model="email" placeholder="Digite o seu e-mail">
        </div>
        <div class="input-container">
            <label for="password">Password:</label>
            <input type="password" name="password" id="password" v-model="password" placeholder="Digite o seu password">
        </div>
        <div class="input-container">
            <label for="confirmPassword">Confirm:</label>
            <input type="password" name="confirmPassword" id="confirmPassword" v-model="confirmPassword" placeholder="Repeat the password">
        </div>
        <InputSubmit :text="btnText"/>
    </div>
</template>

<script>
    import InputSubmit from './form/InputSubmit.vue';
    import Message from './Message.vue';
    export default {
        name: 'ResgisterForm',
        data() {
            return {
                name: null,
                email: null,
                password: null,
                confirmPassword: null,
                btnText: 'Register',
                msg: "Esta é a mensagem",
                msgClass: "success"
            }
        },
        components: {
            InputSubmit,
            Message
        }
    }
</script>

<style scoped>
</style>