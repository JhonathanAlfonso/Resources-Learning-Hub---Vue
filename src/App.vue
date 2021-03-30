<template>
    <the-header
        :title ="'Remember me'"
    ></the-header>
    <stored-resource
        :resources="storedResources"
    ></stored-resource>
</template>

<script>
import TheHeader from './components/layouts/TheHeader.vue'
import StoredResource from './components/learning-resource/StoreResource.vue'
export default {
    components: {
        StoredResource,
        TheHeader
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

<style>
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap');

* {
  box-sizing: border-box;
}

html {
  font-family: 'Roboto', sans-serif;
}

body {
  margin: 0;
}
</style>