<script>
export default {
    name:'TabSection'
}
</script>
<template>
    <div class="row gx-0">
        <div class="col-4 position-relative">
            <img src="../assets/img-un/home_courses_section_bg.jpg" alt="courses">
            <div class="text position-absolute top-50 start-50 translate-middle text-center">
                <h4>COURSES</h4>
                <div class="mini-bar mt-4 mb-3"></div>
                <a href="" >View More</a>
            </div>

        </div><div class="col-4 position-relative">
            <img src="../assets/img-un/home_events_section_bg.jpg" alt="events">
            <div class="text position-absolute top-50 start-50 translate-middle text-center">
                <h4>EVENTS</h4>
                <div class="mini-bar mt-4 mb-3"></div>
                <a href="" >View More</a>
            </div>

        </div>
        <div class="col-4 position-relative">
            <img src="../assets/img-un/home_latest_news_section_bg.jpg" alt="news">
            <div class="text position-absolute top-50 start-50 translate-middle text-center">
                <h4>LATEST NEWS</h4>
                <div class="mini-bar mt-4 mb-3"></div>
                <a href="" >View More</a>
            </div>

        </div>

        
    </div>
</template>
<style scoped lang="scss" >
@use '../style/variables' as *;
img{
    width: 100%;
}
.text{
    color : $color-white
}
.mini-bar {
    width: 50px; 
    height: 1.5px; 
    background-color: $color-orange;
    margin: 0 auto; 
    margin-top: 10px; 
}
</style>