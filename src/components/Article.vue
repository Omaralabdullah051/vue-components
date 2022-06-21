<template>
    <div>
       <h2>Article Component</h2>
       <h2 v-bind="$attrs">{{title}}</h2>
       <h2>Likes -{{likes}}</h2>
       <h2>Published -{{ isPublished ? 'Yes' : 'No' }}</h2>
       <h2>Name - {{object.name}}</h2>
    </div>
</template>

<script>
    export default {
        name: 'ArticleA',
        props: {
            title: {
                type: String,
                required: true,
            },
            likes:{
                type: Number,
                default: 40
            },
            isPublished: Boolean,
            object: Object
        },
        inheritAttrs: false
    }
</script>

<style scoped>

</style>