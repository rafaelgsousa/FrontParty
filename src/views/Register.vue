<script>
    import UserForm from '../components/UserForm.vue';
    export default {
        name: 'Register',
        components: {
            UserForm
        }
    }
</script>

<template>
    <div class="register">
        <h1>Register</h1>
        <UserForm/>
    </div>
</template>

<style scoped>
    .register {
        text-align: center;
        padding-top: 40px;
        padding-bottom: 100px;
    }

    .register h1 {
        margin-bottom: 40px;
    }
</style>
