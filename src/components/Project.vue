<template>
  <a :href="href" class="collection-item waves-effect waves-darken">
    {{ title }}
  </a>
</template>

<script>
export default {
  name: 'project',
  props: ['href', 'title']
};
</script>

<style scoped>
</style>
