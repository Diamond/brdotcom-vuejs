<template>
  <footer class="page-footer red lighten-2">
    <a name="about" />
    <div class="container">
      <div class="row">
        <div class="col s4 white-text">
          <h4>Social Media</h4>
          <div class="row">
            <div class="col s4">
              <a href="https://twitter.com/diamondgfx">
                <i class="fi-social-twitter small">&nbsp;</i>
              </a>
            </div>
            <div class="col s4">
              <a href="https://medium.com/@diamondgfx">
                <i class="fi-social-medium small">&nbsp;</i>
              </a>
            </div>
            <div class="col s4">
              <a href="https://github.com/Diamond">
                <i class="fi-social-github small">&nbsp;</i>
              </a>
            </div>
          </div>
        </div>
        <div class="col s4 white-text">
          <h4>Tech Skills</h4>
          <ul>
            <li>Elixir/Phoenix</li>
            <li>Ruby/Ruby on Rails</li>
            <li>React</li>
            <li>Javascript</li>
            <li>APIs</li>
          </ul>
        </div>
        <div class="col s4 white-text">
          <h4>About Me</h4>
          <p class="">
            I am a software engineer, rubyist, rails...ist, elixirist, and hobbyist
            game developer living in Downstate New York.
            <br /><br />
            When I'm not coding, you can usually find me training in martial arts,
            gaming, or hanging out with my family!
          </p>
        </div>
      </div>
    </div>
    <div class="footer-copyright red lighten-1 bottom-bar">
      <div class="container">
        <div class="row valign-wrapper">
          <div class="col s10">
            © 2017 Brandon Richey // This site was written in React and next.js!
          </div>
          <div class="col s2 right-align">
            <a href="#">Back to top</a>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'custom-footer'
};
</script>

<style scoped>
  .page-footer a { color: white !important; }
  .bottom-bar { padding-top: 20px; padding-bottom: 0px; }
</style>
