<template>
  <input
    type="text"
    :value="modelValue"
    @input="$emit('update:modelValue', $event.target.value)"
  />
</template>

<script>
export default {
  name: 'InputA',
  props: {
    modelValue: String,//will automatically receive the prop because we use v-model on custom component
  },
  emits: ['update:modelValue'],
}
</script>

<style scoped>
input[type='text'] {
  display: block;
  width: 400px;
  padding: 6px 12px;
  font-size: 14px;
  line-height: 1.4;
  color: #555;
  background-color: #fff;
  background-image: none;
  border: 1px solid #ccc;
  border-radius: 4px;
}
</style> 
0 comments on c