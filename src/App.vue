<script>
import AppHeader from './components/AppHeader.vue'
  export default {
    components : {
      AppHeader

    },
    data() {
    return {
        contacts: [
            {
                'number': "1.800.654.125.452",
                'email': "Contact Us",
                "alumn": "Alumni",
                "campus": "Campus" , 
                "fb" : '<i class="fa-brands fa-facebook-f"></i> ',
                "twitter" : '<i class="fa-brands fa-twitter"></i>',
                "yt" :'<i class="fa-brands fa-youtube"></i>',
                "insta" : '<i class="fa-brands fa-instagram"></i>'
                
            },
            
            ],

        
        }         
    }
}
  
</script>

<template>
  <header>
    <AppHeader v-for="contact in contacts " :contactInfo="contact"> </AppHeader>
  </header>
</template>

<style lang="scss">
 @use './style/generic'

</style>
