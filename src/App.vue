<template>
    <resource-item 
        v-for="resource in storedResources" 
        :key="resource.id"
        :title="resource.title"
        :description="resource.description"
        :link="resource.link"
    ></resource-item>
</template>

<script>
import ResourceItem from './components/LearningResource/ResourceItem.vue'
export default {
    components: {
        ResourceItem
    },

    data() {
        return {
            storedResources: [
                { 
                    id: 'official-guide', 
                    title: 'Official Guide',
                    description: 'The official Vue.js docs',
                    link: 'https://vuejs.org'
                 },
                 { 
                    id: 'google', 
                    title: 'Google',
                    description: 'Google source',
                    link: 'https://google.com'
                 }
            ]
        }
    },
}
</script>