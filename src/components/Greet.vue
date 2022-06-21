<template>
    <h2>
        Hello {{name}} | {{heroName}}
    </h2>
</template>

<script>
    export default {
        name: 'GreetA',
        props: ['name', 'heroName']
    }
</script>

<style scoped>
</style>
