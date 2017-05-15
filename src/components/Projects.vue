<template>
  <div class="section container">
    <a name="projects" />
    <h5>My Favorite Projects</h5>
    <div class="collection">
      <project v-for="project in projects" :key="project.href" :href="project.href" :title="project.title" />
    </div>
  </div>
</template>

<script>
import Project from './Project';

export default {
  name: 'projects',
  components: {
    Project
  },
  data() {
    return {
      projects: [
        {
          href: 'https://github.com/Diamond/pxblog',
          title: 'Elixir/Phoenix Blog Project'
        },
        {
          href: 'https://github.com/Diamond/elm_articles',
          title: 'Elm Articles'
        },
        {
          href: 'https://github.com/Diamond/livechat-elm',
          title: 'Elm/Phoenix Websockets Chat App'
        },
        {
          href: 'https://github.com/Diamond',
          title: 'Find more on GitHub!'
        }
      ]
    };
  }
};
</script>

<style scoped>

</style>
