<script>
import AppAccordion from './AppAccordion.vue'
import TabSection from './TabSection.vue'
import AppCard from './AppCard.vue'
import AppRegistration from './AppRegistration.vue'
export default {
    name: 'AppMain',
    components : {
        AppAccordion,
        TabSection,
        AppCard ,
        AppRegistration
    }
}
</script>

<template>

    <div class="introduction-section">
        <div class="text-center mt-4 py-4">
            <img src="../assets/img-un/page-logo-1.png" alt="logo">
            <h3 class="mt-3">Inspirng by Excellence & Innovation</h3>
            <p class="p-large">We offer a wide range of high quality of teaching and extra-curricular activities</p>
            <div class="mini-bar"></div>
        </div>
        <div class="ms-container mt-3">
            <div class="row g-0">
                <div class="col-8">
                    <h5>WHY CHOOSE AVADA UNIVERSITY</h5>
                    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Labore delectus fuga eum quidem alias, nam iusto eius nisi possimus harum incidunt porro omnis, fugit dolorum enim cum laborum voluptatibus ipsa. Lorem ipsum dolor sit amet
                        consectetur, adipisicing elit. Iure necessitatibus, asperiores, consequatur nostrum, placeat tenetur omnis ab totam quo molestiae porro harum sit reprehenderit. Error, id? Vel rem deserunt provident?</p>
                    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ex possimus iure sint tenetur veniam distinctio voluptate sapiente error! Nesciunt, non velit modi ipsa esse dignissimos voluptates eum at voluptas tempora.</p>
                </div>
                <div class="col-4 d-flex align-items-center justify-content-center ">
                    <img class="" src="../assets/img-un/politics_seminar_event_feat-600x402.jpg" alt="#">
                </div>
            </div>

        </div>
    </div>

    <div class="facilities-and-values-section py-5">
        <div class="ms-container ">
            <div class="row d-flex  ">
                <div class="col-6 mt-5">
                    <h5>  WORLD CLASS FACILITIES</h5>
                    <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Molestiae corrupti assumenda nostrum voluptates, tempora quis minus nam asperiores? Molestiae ipsum amet pariatur! Suscipit eligendi eaque iusto, fugit quos nostrum nemo!</p>
                    <div class="mt-4 p-2">
                        <div class="d-flex gap-2 align-items-center">
                            <i class="fa-solid fa-globe me-3"></i>
                            <h5> International focus -</h5>
                            <p class="mb-2"> our students come from across the globe</p>
                        </div>
                        <div class="d-flex gap-2 align-items-center ">
                            <i class="fa-solid fa-graduation-cap me-2"></i>
                            <h5 class="ms-1"> Residential courses -</h5>
                            <p class="mb-2">we encourage learning and growth - </p>
                        </div>
                        <div class="d-flex gap-2 align-items-center">
                            <i class="fa-regular fa-address-book me-3"></i>
                            <h5>People not profits - </h5>
                            <p class="mb-2"> education is a right not a privilage</p>
                        </div>
                    </div>
                    <p class="mt-3">Lorem ipsum dolor sit amet consectetur, adipisicing elit. Eius ab ut omnis quo consectetur vero repellendus</p>
                </div>
                <div class="col-6 mt-5">
                    <h5>OUR VALUES</h5>
                    <!-- SECTION ACCORDION YOU CAN FIND IT IN COMPONENTS TAPPACCORDION.VUE -->
                    <AppAccordion class="mt-3"></AppAccordion>
                </div>
            </div>
        </div>
    </div>
    
    <!-- SECTION TAB YOU CAN FIND IT IN COMPONENTS TABSECTION.VUE -->
    <TabSection></TabSection>

    <div class="foot-main mt-5">
        <div class="text-center">
            <img src="../assets/img-un/page-logo-1.png" alt="">
            <h4 class="mt-4">Today's University News</h4>
            <p class="mt-2">Covering topics from classes to politics and student organization event </p>
            <div class="mini-bar my-5"></div>
        </div>
        <!-- SECTION CARD YOU CAN FIND IT IN COMPONENTS APPCARD.VUE -->
       <AppCard class="mb-5"></AppCard>   

    </div>
    <!-- SECTION REGISTRATION YOU CAN FIND IT IN COMPONENTS REGISTRATION.VUE -->

    <AppRegistration></AppRegistration>
</template>

<style scoped lang="scss">
@use '../style/variables' as *;
.mini-bar {
    width: 150px; 
    height: 1.5px; 
    background-color: $color-orange;
    margin: 0 auto; 
    margin-top: 10px; 
}

.p-large{
    font-size: 18px;
}

.ms-container{
    img{
        width: 100%;
        height: 80%;
        object-fit: cover;
    }
}

.bottom{
    margin-top: 250px;
    background: $color-white-2;
   
}
p{
    font-size: 13px;
    color : $color-gray
}

.col-6{
    p{
        line-height: 1.7;
    }
}

h5,h3{
    color : $color-gray-d;
}
h5{
    font-size: 18px;
}
h3{
    font-size: 27px;
}

i{
    color : $color-orange;
   font-size: 20px;
}

.foot-main{
    p{
        font-size: 20px;
    }
}

</style>











    
