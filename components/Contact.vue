<template>
  <div id="contactUs" class="the-container contact-container">
    <div class="container">
      <div class="big-title">
        {{bigTitle}}
      </div>
      <p class="section-title__text">
        Let&apos;s get in touch
      </p>
      <div class="contact-content">
        <p class="body-text text-center">
          Just want to say hello, I&apos;ll try my best to get back to you!
        </p>

        <div class="contact-btn text-center">
          <a href="mailto:lemuelpaconlloren@gmail.com" class="btn primary-button">Say Hello</a>
        </div>
      </div>
      <div class="social-medias">
        <p class="project-title text-center mb-4">Follow me on</p>
        <!-- social media  -->
        <!-- icons  -->
        <div class="techstack--icons d-flex justify-content-center">
          <ul class="my-icons-ul d-flex">
            <li class="my-icons-li">
              <a href="#">
                <div class="my-icons-wrap">
                  <span class="fab fa-facebook-f my-icons-lg"></span>
                  <span class="my-icons-wrap__text">Facebook</span>
                </div>
              </a>
            </li>
            <li class="my-icons-li">
              <a href="#">
                <div class="my-icons-wrap">
                  <span class="fab fa-instagram my-icons-lg"></span>
                  <span class="my-icons-wrap__text">Instagram</span>
                </div>
              </a>
            </li>
            <li class="my-icons-li">
              <a href="#">
                <div class="my-icons-wrap">
                  <span class="fab fa-github my-icons-lg"></span>
                  <span class="my-icons-wrap__text">Github</span>
                </div>
              </a>
            </li>
            <li class="my-icons-li">
              <a href="#">
                <div class="my-icons-wrap">
                  <span class="fab fa-dribbble my-icons-lg"></span>
                  <span class="my-icons-wrap__text">Dribbble</span>
                </div>
              </a>
            </li>
            <li class="my-icons-li">
              <a href="#">
                <div class="my-icons-wrap">
                  <span class="fab fa-behance my-icons-lg"></span>
                  <span class="my-icons-wrap__text">Behance</span>
                </div>
              </a>
            </li>
          </ul>
        </div>
        <!-- icons  -->
        <!-- social media  -->
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        bigTitle: 'Contact'
      }
    }
  }

</script>
