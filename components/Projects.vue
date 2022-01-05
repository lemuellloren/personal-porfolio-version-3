<template>
  <div class="experience-container">
    <div class="container">
      <div class="big-title">
        {{bigTitle}}
      </div>
      <p class="section-title__text">
        A glance of all projects I&apos;ve built
      </p>
      <div class="projects">
        <!-- project template  -->
        <div class="row d-flex align-items-center projects__template">
          <div class="col-lg-5">
            <p class="project-title d-flex justify-content-between">Project name<NuxtLink class="icon-link" to="/"><i
                  class="fas fa-external-link-alt"></i></NuxtLink>
            </p>
            <p class="body-text">
              Amet minim mollit non deserunt ullamco est sit aliqua dolor do amet sint.
            </p>
            <div class="projects__tags d-flex">
              <div class="body-text-lg tags">Web Development</div>
              <div class="body-text-lg tags">UX/UI</div>
            </div>
            <!-- icons  -->
            <div class="projects__stacks techstack--icons">
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
              </ul>
            </div>
            <!-- icons  -->
          </div>
          <div class="col-lg-7">
            <div class="projects__img-wrap">
              <img src="images/project-sample.png" alt="Project 1">
            </div>
          </div>
        </div>
        <!-- project template  -->
        <!-- project template invert  -->
        <div class="row d-flex align-items-center projects__template">
          <div class="col-lg-7">
            <div class="projects__img-wrap">
              <img src="images/project-sample.png" alt="Project 1">
            </div>
          </div>
          <div class="col-lg-5">
            <p class="project-title d-flex justify-content-between">Project name<NuxtLink class="icon-link" to="/"><i
                  class="fas fa-external-link-alt"></i></NuxtLink>
            </p>
            <p class="body-text">
              Amet minim mollit non deserunt ullamco est sit aliqua dolor do amet sint.
            </p>
            <div class="projects__tags d-flex">
              <div class="body-text-lg tags">Web Development</div>
              <div class="body-text-lg tags">UX/UI</div>
            </div>
            <!-- icons  -->
            <div class="projects__stacks techstack--icons">
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
              </ul>
            </div>
            <!-- icons  -->
          </div>
        </div>
        <!-- project template invert  -->
        <!-- project template  -->
        <div class="row d-flex align-items-center projects__template">
          <div class="col-lg-5">
            <p class="project-title d-flex justify-content-between">Project name<NuxtLink class="icon-link" to="/"><i
                  class="fas fa-external-link-alt"></i></NuxtLink>
            </p>
            <p class="body-text">
              Amet minim mollit non deserunt ullamco est sit aliqua dolor do amet sint.
            </p>
            <div class="projects__tags d-flex">
              <div class="body-text-lg tags">Web Development</div>
              <div class="body-text-lg tags">UX/UI</div>
            </div>
            <!-- icons  -->
            <div class="projects__stacks techstack--icons">
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
              </ul>
            </div>
            <!-- icons  -->
          </div>
          <div class="col-lg-7">
            <div class="projects__img-wrap">
              <img src="images/project-sample.png" alt="Project 1">
            </div>
          </div>
        </div>
        <!-- project template  -->
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        bigTitle: 'Projects'
      }
    }
  }

</script>
