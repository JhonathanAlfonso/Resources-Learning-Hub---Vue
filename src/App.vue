<template>
    <ul></ul>        
</template>

<script>
export default {
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