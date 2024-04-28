<script>
import AppHeader from './components/AppHeader.vue'
import AppHero from './components/AppHero.vue'
import AppMain from './components/AppMain.vue'
import AppFooter from './components/AppFooter.vue'
  export default {
    components : {
      AppHeader ,
      AppHero , 
      AppMain , 
      AppFooter
      

    },
    data() {
    return {
        socials: [
            {
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
    <AppHeader v-for="social in socials " :socialInfo=social>
      
    </AppHeader>
    <AppHero></AppHero>
  </header>
  <main>
    //  <!-- first section of main -->
    <section>
      <AppMain ></AppMain>
    </section>
     <!--///// first section of main -->
  </main>

  <footer>
    <!-- footer -->
    <AppFooter v-for="social in socials " :socialInfo=social></AppFooter>
  </footer>
</template>


<style lang="scss">
 @use './style/generic'

</style>
  

 
    
 

