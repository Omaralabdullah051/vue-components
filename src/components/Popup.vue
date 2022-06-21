<template>
    <div>
       <h2>This is a popup</h2>
       <button @click="$emit('close','Clark')">Close popup</button>
    </div>
</template>

<script>
    export default {
        name:'PopupA',
        emits: ['close']
    }
</script>

<style scoped>

</style>