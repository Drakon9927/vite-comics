<script>
export default {
    data() {
        return {
            message: "Benvenuto nella sezione principale"
        }
    }
}
</script>

<template>
    <main>
        <p>{{ message }}</p>
    </main>
</template>

<style scoped>
main {
    background-color: #eee;
    padding: 1rem;
    text-align: center;
}
</style>