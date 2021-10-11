<template>
   <div class="the-footer d-flex justify-content-center align-items-center">
       <div class="container">
           <div class="footer-text">
               Made with 💜 by <span class="footer-text__creator-name">Lemuel Lloren</span>
           </div>
            <div class="footer-text">
              Copyright {{date}}
           </div>
       </div>
   </div>
</template>

<script>
export default {
  data() {
    return {
      date: new Date().getFullYear()
    }
  }
}
</script>