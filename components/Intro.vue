<template>
  <div class="intro-container">
    <div class="container">
      <div class="intro text-center">
        <div class="big-title">
          {{ bigTitle }}
        </div>
        <h1 class="intro__heading">
          Hello, Amigo!
        </h1>
        <h3 class="intro__subheading">
          I’m Lemuel a <span class="intro__subheading--bold">Software Developer</span>
        </h3>
        <p class="intro__body">
          I like to craft solid and scalable frontend products with great user experiences.
        </p>
        <div class="intro__btn-group pt-3">
          <a href="#" class="btn primary-button mr-3">Portfolio</a>
          <a href="#" class="btn secondary-button mr-3">Resume</a>
        </div>
        <!-- Technology and Tools  -->
        <div class="techstack">
          <div class="section-title">
            <div class="big-title">
              Techstack
            </div>
            <p class="section-title__text">
              Technologies &amp; Tools
            </p>
            <p class="body-text">
              Here are a few technologies &amp; tools I’ve been working with recently:
            </p>
          </div>
          <!-- icons  -->
          <div class="techstack--icons d-flex justify-content-center">
            <ul class="my-icons-ul d-flex">
              <li class="my-icons-li">
                <div class="my-icons-wrap">
                  <span class="fab fa-js-square my-icons-lg"></span>
                  <span class="my-icons-wrap__text">JavaScript (ES6+)</span>
                </div>
              </li>
              <li class="my-icons-li">
                <div class="my-icons-wrap">
                  <span class="fab fa-angular my-icons-lg"></span>
                   <span class="my-icons-wrap__text">Angular</span>
                </div>
              </li>
              <li class="my-icons-li">
                <div class="my-icons-wrap">
                  <span class="fab fa-vuejs my-icons-lg"></span>
                  <span class="my-icons-wrap__text">VueJS</span>
                </div>
              </li>
              <li class="my-icons-li">
                <div class="my-icons-wrap">
                  <span class="fab fa-react my-icons-lg"></span>
                  <span class="my-icons-wrap__text">ReactJS</span>
                </div>
              </li>
              <li class="my-icons-li">
                <div class="my-icons-wrap">
                  <span class="fab fa-php my-icons-lg"></span>
                  <span class="my-icons-wrap__text">PHP</span>
                </div>
              </li>
              <li class="my-icons-li">
                <div class="my-icons-wrap">
                  <span class="fab fa-wordpress-simple my-icons-lg"></span>
                  <span class="my-icons-wrap__text">WordPress</span>
                </div>
              </li>
              <li class="my-icons-li">
                <div class="my-icons-wrap">
                  <span class="fab fa-laravel my-icons-lg"></span>
                  <span class="my-icons-wrap__text">Laravel</span>
                </div>
              </li>
              <li class="my-icons-li">
                <div class="my-icons-wrap">
                  <span class="fab fa-figma my-icons-lg"></span>
                  <span class="my-icons-wrap__text">Figma</span>
                </div>
              </li>
            </ul>
          </div>
          <!-- icons  -->
        </div>
        <!-- Technology and Tools  -->
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        bigTitle: 'awesome'
      }
    }
  }

</script>
