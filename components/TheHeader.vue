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
                        <NuxtLink class="menu__link fas fa-home switch-theme__icon" to="/"></NuxtLink>
                   </li>
                   <li class="menu__list">
                       <NuxtLink class="menu__link" to="/">About Me</NuxtLink>
                   </li>
                   <li class="menu__list">
                       <NuxtLink class="menu__link" to="/">Experience</NuxtLink>
                   </li>
                   <li class="menu__list">
                        <a href="#"><span class="fas fa-sun switch-theme-icon"></span></a>
                   </li>
               </ul>
           </nav>
       </div>
      </div>
    </div>
  </header>
</template>
