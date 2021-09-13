<template>
  <header class="the-header d-flex justify-content-center align-items-center">
    <div class="container">
      <div class="row">
       <div class="col-lg-6">
            <div class="logo">
          lemuel<span>lloren</span>
        </div>
       </div>
       <div class="col-lg-6 d-flex justify-content-end align-items-center">
           <nav class="nav">
               <ul class="menu">
                   <li class="menu__list">
                        <NuxtLink class="menu__link" to="/">Projects</NuxtLink>
                   </li>
                   <li class="menu__list">
                       <NuxtLink class="menu__link" to="/">Snippets</NuxtLink>
                   </li>
                   <li class="menu__list">
                       <NuxtLink class="menu__link" to="/">Contact Me</NuxtLink>
                   </li>
               </ul>
           </nav>
           <div class="switch-theme">
               <a href="#"><span class="fas fa-sun switch-theme__icon"></span></a>
           </div>
       </div>
      </div>
    </div>
  </header>
</template>
