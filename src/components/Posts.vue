<template>
  <div class="section container">
    <a name="posts" />
    <h5>Noteworthy Posts</h5>
    <div class="collection">
      <post v-for="post in posts" :key="post.href" :href="post.href" :title="post.title" />
    </div>
  </div>
</template>

<script>
import Post from './Post';

export default {
  name: 'posts',
  components: {
    Post
  },
  data() {
    return {
      posts: [
        {
          href: 'https://medium.com/@diamondgfx/nextjs-lessons-learned-part-1-a5a8d442450f',
          title: 'Lessons Learned Building in Next.js (Series)'
        },
        {
          href: 'https://medium.com/@diamondgfx/learning-react-with-create-react-app-part-1-a12e1833fdc',
          title: 'Learning React with Create-React-App (Series)'
        },
        {
          href: 'https://hackernoon.com/introduction-fe138ac6079d',
          title: 'Writing a Blog Engine in Phoenix and Elixir (Series)'
        },
        {
          href: 'https://medium.com/@diamondgfx',
          title: 'Find more on Medium!'
        }
      ]
    };
  }
};
</script>

<style scoped>

</style>
