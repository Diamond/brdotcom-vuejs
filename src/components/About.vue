<template>
  <div class="big-bg valign-wrapper">
    <div class="valign-wrapper overlay">
      <h5 class="row center-align red-text text-lighten-1">
        What Do I Do?
      </h5>
      <h5 class="row center-align">
        {{ makeSkills() }}
      </h5>
    </div>
  </div>
</template>

<script>
export default {
  name: 'about',
  data() {
    return {
      skills: ['Elixir', 'React', 'Ruby', 'JavaScript', 'Games', 'Martial Arts'],
      accentColor: 'red-text'
    };
  },
  methods: {
    makeSkills() {
      return this.skills.join(', ');
    }
  }
};
</script>

<style scoped>
  .big-bg {
    background-image: url('/static/images/about-header.jpg');
    background-size: cover;
    color: white;
    min-height: 400px;
    height: 400px;
    width: 100%;
  }
  .overlay {
    position: relative;
    width: 100%;
    height: 100%;
    background-color: rgba(0, 0, 0, 0.75);
  }
</style>
