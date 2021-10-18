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
  //* VARIABLES
  $primary-color: #7D5FFF;
  $secondary-color: #1A202C;
  $white: #F7F7F7;
  $dark-bg: #1D2430;
  $body-text: 18px;
  $body-text-md: 12px;
  $big-title: 90px;
  $section-title: 30px;
  $project-title: 24px;
  $box-shadow: 0px 10px 10px rgba(0, 0, 0, 0.1);
  $border-radius: 5px;
  $border-hover: 2px solid $primary-color;
  $font: 'Poppins',
  sans-serif;
  $transitions: all ease .4s;
  $border: 2px solid $primary-color;
  $body-line-height: 1.5em;
  $heading-line-height: 1em;
  $bold: bold;

  //* MIXINS
  // menu 
  @mixin menu-link {
    font-size: 14px;
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
    background-color: $secondary-color;
    min-height: 880px;
    padding-top: 20px;
    padding-bottom: 20px;
  }

  // heading 
  @mixin heading {
    color: $white;
    font-weight: 500;
    line-height: $heading-line-height;
  }

  // body text 
  @mixin body-text {
    font-weight: normal;
    font-size: $body-text;
    line-height: $body-line-height;
    color: $white;
  }

  // primary button 
  @mixin primary-btn {
    z-index: 1;
    position: relative;
    color: $secondary-color;
    font-size: 18px;
    font-style: normal;
    font-weight: 500;
    border-radius: $border-radius;
    transition: $transitions;
    background-color: $primary-color;
    border: 2px solid $primary-color;

    &::before {
      content: '';
      z-index: -1;
      position: absolute;
      top: 0;
      bottom: 0;
      left: 0;
      right: 0;
      background-color: $secondary-color;
      border-radius: $border-radius;
      transform-origin: center bottom;
      transform: scaleY(0);
      transition: transform 0.25s ease-in-out;
    }

    &:hover {
      cursor: pointer;
      color: $white;
    }

    &:hover::before {
      transform-origin: center top;
      transform: scaleY(1);
    }
  }

  // secondary button 
  @mixin secondary-btn {
    z-index: 1;
    position: relative;
    color: $primary-color;
    font-size: 18px;
    font-style: normal;
    font-weight: 500;
    background: unset;
    border: 2px solid $primary-color;
    border-radius: $border-radius;

    &::before {
      content: '';
      z-index: -1;
      position: absolute;
      top: 0;
      bottom: 0;
      left: 0;
      right: 0;
      background-color: $primary-color;
      transform-origin: center bottom;
      transform: scaleY(0);
      transition: transform 0.25s ease-in-out;
    }

    &:hover {
      cursor: pointer;
      color: $white;
    }

    &:hover::before {
      transform-origin: center top;
      transform: scaleY(1);
    }
  }


  //* GLOBAL CLASS 
  .body-text {
    @include body-text;
    padding-bottom: 30px;
  }

  // icons 
  .my-icons-lg {
    color: $white;
    font-size: 30px;
    width: 72px;
    height: 72px;
    background: $dark-bg;
    box-shadow: $box-shadow;
    border-radius: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
    margin: 10px;
    transition: $transitions;

    &:hover {
      border: $border-hover;
      color: $primary-color;
    }
  }

  // icon tooltip 
  .my-icons-wrap {
    position: relative;
    display: flex;
    justify-content: center;
    align-content: center;

    &__text {
      position: absolute;
      top: 60%;
      margin-top: 10px;
      padding: 10px;
      font-weight: 500;
      color: $white;
      font-size: $body-text-md;
      background: $secondary-color;
      border: $border;
      box-sizing: border-box;
      border-radius: $border-radius;
      white-space: nowrap;
      pointer-events: none;
      user-select: none;
      opacity: 0;
      transition: all 0.2s ease-in-out;
    }

    &:hover {
      span {
        top: 100%;
        opacity: 0.9;
      }
    }
  }

  // icons list 
  .my-icons-ul {
    padding: 0;
    list-style: none;
    margin: 0;
  }

  // buttons 
  .primary-button {
    @include primary-btn;
  }

  .secondary-button {
    @include secondary-btn;
  }

  // section title 
  .section-title {
    &__text {
      color: $white;
      font-weight: 500;
      font-size: 30px;
      line-height: $heading-line-height;
      position: relative;
      margin-top: -55px;
      margin-bottom: 50px;

      &:after {
        content: '';
        height: 5px;
        width: 70px;
        position: absolute;
        background-color: $primary-color;
        left: 0;
        right: 0;
        bottom: -15px;
        margin: 0 auto;
      }
    }
  }


  // * GLOBAL STYLES 
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

  // Big title 
  .big-title {
    color: $dark-bg;
    font-size: $big-title;
    font-weight: 900;
    text-align: center;
    line-height: 8.4375rem;
    letter-spacing: 0.24em;
    text-transform: uppercase;
  }

  //* Intro Section 
  .intro-container {
    @include section-default;

    .intro {
      &__heading {
        @include heading;
        font-size: 90px;
        font-weight: $bold;
        margin-top: -70px;
      }

      &__subheading {
        @include heading;
        margin-top: 20px;
      }

      &__subheading--bold {
        color: $primary-color;
        font-weight: 600;
      }

      &__body {
        @include body-text;
        width: 45%;
        margin: 0 auto;
        padding-bottom: 30px;
      }
    }
  }

  //* Technology Tools 
  .techstack {
    padding-top: 100px;
  }

  // * Footer 
  .the-footer {
    min-height: 120px;
    background-color: $secondary-color;
    // position: absolute;
    // bottom: 0;
    // width: 100%;

    .footer-text {
      @include body-text;
      text-align: center;

      &__creator-name {
        font-weight: 500;
        color: $primary-color;
      }
    }
  }

</style>
