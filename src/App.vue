<template>
  <the-header title="Learning Resources" />
  <stored-resources :resources="storedResources" />
</template>

<script>
import TheHeader from './components/layout/TheHeader.vue';
import StoredResources from './components/learning-resources/StoredResources.vue';

export default {
  components: {
    StoredResources,
    TheHeader,
  },
  data() {
    return {
      storedResources: [
        {
          id: 'official-guide',
          title: 'Official Guide',
          description: 'The official documentation for Vue.js 3',
          link: 'https://vuejs.org',
        },
        {
          id: 'google',
          title: 'Google',
          description: "It's Google!",
          link: 'https://google.com',
        },
      ],
    };
  },
};
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
