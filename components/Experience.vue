<template>
  <div class="experience-container">
    <div class="container">
      <div class="big-title">
        {{bigTitle}}
      </div>
      <p class="section-title__text">
        Where Have I Worked Before?
      </p>
      <div class="experience-tabs-container">
    <b-card class="global-tabs--card" no-body>
        <b-tabs class="global-tabs" vertical>
            <b-tab title="ViewQwest" active>
                <b-card-text>
                    <div class="experience-tab--pane-content">
                        <p class="project-title">Software Engineer at <span class="project-title-span">ViewQwest Pte Ltd</span>
                        </p>
                        <div class="meta">
                            September 2019 - Present
                        </div>
                        <ul class="global-ul">
                            <li class="global-ul--li">
                                <p class="body-text">
                                    Write code that is modern, performant, and maintainable for a wide range of client and
                                    internal projects.
                                </p>
                            </li>
                            <li class="global-ul--li">
                                <p class="body-text">
                                    Work with a wide range of languages, platforms, frameworks, and content management systems,
                                    including JavaScript, TypeScript, Angular, VueJS, Laravel, and WordPress.
                                </p>
                            </li>
                            <li class="global-ul--li">
                                <p class="body-text">
                                    On a daily basis, communicate with multidisciplinary teams of engineers, project owners, and
                                    designers.
                                </p>
                            </li>
                        </ul>
                    </div>
                </b-card-text>
            </b-tab>
            <b-tab title="TechRemote">
                <b-card-text>Tab contents 2</b-card-text>
            </b-tab>
            <b-tab title="Leet Digital">
                <b-card-text>Tab contents 3</b-card-text>
            </b-tab>
        </b-tabs>
    </b-card>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        bigTitle: 'Experience'
      }
    }
  }

</script>
