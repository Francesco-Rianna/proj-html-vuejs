<script>
export default {
    name : 'AppHeader' ,
    props : {
        contactInfo : Object
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
                        <li> <i class="fa-solid fa-phone-flip"></i> {{ contactInfo.number }}</li>
                        <li> <i class="fa-solid fa-envelope"></i> {{ contactInfo.email}}</li>
                        <li> <i class="fa-solid fa-graduation-cap"></i> {{ contactInfo.alumn}}</li>
                        <li> <i class="fa-solid fa-building-columns"></i> {{ contactInfo.campus}}</li>
                    </ul>
                   </nav>
                </div>
                <div class="right">
                    <nav>
                    <ul class="d-flex list-unstyled gap-3 ">
                        <li v-html="contactInfo.fb"></li>
                        <li v-html="contactInfo.twitter"></li>
                        <li v-html="contactInfo.yt"></li>
                        <li v-html="contactInfo.insta"></li>
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
                    <a href=""><li>HOME</li> </a>
                    <a href=""><li>ABOUT</li></a>
                    <a href=""><li>COURSES</li></a>
                    <a href=""><li>EVENTS</li></a>
                    <a href=""><li>FACILITIES</li></a>
                    <a href=""><li>NEWS</li></a>
                    <a href=""><li>ADMISSIONS</li></a> 
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