<template>
  <nav>
    <div class="nav-wrapper blue-grey darken-3 top-bar">
      <a href="#" class="brand-logo top-logo">
        {{ unaccented }}<span :class="accentClasses()">{{ accented }}</span>
      </a>
      <ul id="nav-mobile" class="right">
        <li v-for="link in links">
          <a v-bind:href="makeHref(link)" class="center waves-effect waves-red">
            {{ link }}
          </a>
        </li>
      </ul>
    </div>
  </nav>
</template>

<script>
export default {
  name: 'nav-bar',
  data() {
    return {
      links: ['Posts', 'Projects', 'Presentations', 'About'],
      unaccented: 'brandon',
      accented: '.richey',
      accentColor: 'red-text'
    };
  },
  methods: {
    makeHref(link) {
      return `#${link.toLowerCase()}`;
    },
    accentClasses() {
      return `${this.accentColor} text-lighten-1`;
    }
  }
};
</script>

<style scoped>
  .top-bar { margin-bottom: 1px; }
  .top-logo { margin-left: 20px; }
</style>
