<template>
  <div class="main-container">
    <TheHeader></TheHeader>
    <Intro></Intro>
    <TheFooter></TheFooter>
  </div>
</template>

<script>
  export default {}

</script>

<style lang="scss">
  //* Variables 
  $primary-color: #7D5FFF;
  $secondary-color: #1A202C;
  $white: #F7F7F7;
  $dark-bg: #1D2430;
  $body-text: 18px;
  $section-title: 30px;
  $project-title: 24px;
  $box-shadow: 0px 10px 10px rgba(0, 0, 0, 0.1);
  $border-radius: 10px;
  $font: 'Poppins',
  sans-serif;
  $transitions: all ease .4s;

  //* Mixins 
  // menu 
  @mixin menu-link {
    font-size: 18px;
    color: $white;
    text-decoration: none;
    transition: $transitions;

    &:hover {
      color: $primary-color;
    }
  }

  body {
    font-family: $font;
  }

  a {
    &:hover {
      text-decoration: none;
    }
  }

  // section default style
  @mixin section-default {
    background-color:  $secondary-color;
     padding-top: 80px;
  padding-bottom: 80px;
  }

  // heading 
  @mixin heading {
    color: $white;
    font-weight: 500;
    line-height: 1em;
  }
  // body text 
  @mixin body-text {
    font-size: 18px;
    line-height: 1.5em;
    color: $white;
    font-weight: normal;
  }
  //* Global Class 
  .my-icons {
    color: $white;
    font-size: 30px;
  }

  //* Header
  .the-header {
    min-height: 120px;
    background-color: $secondary-color;
  }

  .logo {
    color: $white;
    font-weight: 300;
    font-size: 30px;
    line-height: 45px;

    span {
      color: $primary-color;
      font-weight: 500;
      font-size: 30px;
      line-height: 45px;
    }
  }

  .menu {
    list-style: none;
    padding: 0;
    margin: 0;

    &__list {
      margin: 0 10px;
      padding: 0;
      display: inline-block;
    }

    &__link {
      @include menu-link;
    }
  }

  .switch-theme-icon {
    margin-left: 40px;
    @include menu-link;
  }

//* Intro Section 
.intro-container {
  @include section-default;
  .intro {
    &__heading {
     @include heading
    }
  }
}
</style>
