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
                "campus": "Campus"
            },
            
            ],

        social: [
          {
            'fb' : '',
            'twitter': '',
            'yt' :'',
            'insta' :''

          }
        ]
        }         
    }
}
  
</script>

<template>
  <AppHeader> </AppHeader>
</template>

<style lang="scss">
 @use './style/generic'

</style>
