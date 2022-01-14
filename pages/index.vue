<template>
  <div class="main-container">
    <TheHeader></TheHeader>
    <Intro></Intro>
    <Experience></Experience>
    <Projects></Projects>
    <Contact></Contact>
    <TheFooter></TheFooter>
  </div>
</template>

<script>
  import Experience from '../components/Experience.vue'
  export default {
    components: {
      Experience
    },
  }

</script>

