<script>
export default {
    name : 'AppHeader' ,
    props : {
        socialInfo : Object , 
       
    },
    data() {
        return {
            links: [
                { text: "HOME" },
                { text: "ABOUT" },
                { text: "COURSES" },
                { text: "EVENTS" },
                { text: "FACILITIES" },
                { text: "NEWS" },
                { text: "ADMISSIONS" }
            ]
        };

    
 }
}
</script>

<template>
    <div class="bg-header">
        <div class="ms-container">
            <div class="d-flex justify-content-between align-items-center p-1">
                <div class="left">
                   <nav>
                    <ul class="d-flex list-unstyled gap-2">
                        <li> <i class="fa-solid fa-phone-flip"></i> 1.800.654.125.452</li>
                        <li> <i class="fa-solid fa-envelope"></i> Contact Us</li>
                        <li> <i class="fa-solid fa-graduation-cap"></i> Alumni</li>
                        <li> <i class="fa-solid fa-building-columns"></i>Campus</li>
                    </ul>
                   </nav>
                </div>
                <div class="right">
                    <nav>
                       <ul class="d-flex list-unstyled gap-3 ">
                         <a href=""> <li v-html="socialInfo.fb"></li></a>
                         <a href=""><li v-html="socialInfo.twitter"></li></a>
                         <a href=""><li v-html="socialInfo.yt"></li></a>
                         <a href=""><li v-html="socialInfo.insta"></li></a>
                        </ul>
                    </nav>
                    

                </div>
            </div>
        </div>
    </div>

    <div class="ms-container py-4 d-flex justify-content-between align-items-center">
        <div class="left">
            <img src="../assets/img-un/university_logo.png" alt="logo">
        </div>
        
        <div class="right">
            <nav>
                <ul class="d-flex gap-3 list-unstyled ">
                    <a href="" v-for="link in links"> <li>{{ link.text }}</li> </a>
                    
                </ul>
            </nav>
        </div>

    </div>
        
        


</template>

<style scoped lang="scss">
 @use '../style/variables' as *;
.bg-header{
    background-color: $color-orange;
    li {
    color : $color-white;
}
}
</style>