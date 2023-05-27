<template>
    <footer>
        <h3>Party Time &copy; 2021</h3>
        <p>O melhor local para conpartilhar seus eventos!</p>
    </footer>
</template>

<script>
    export default {
        name: 'Footer'
    }
</script>

<style scoped>
    footer {
        background-color: #25282e;
        height: 300px;
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;
    }

    footer h3 {
        color: #fff;
        margin-bottom: 15px;
        font-weight: 300;
        font-size: 1.6rem;
    }

    footer p {
        color: #c1b696
    }
</style>