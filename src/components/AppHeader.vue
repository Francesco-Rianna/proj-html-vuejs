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


</template>

<style scoped lang="scss">
 @use '../style/variables' as *;
.bg-header{
    background-color: $color-orange;
} li {
    color : $color-white;
}
</style>