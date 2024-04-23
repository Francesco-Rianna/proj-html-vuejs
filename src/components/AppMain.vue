<script>
export default {
    name: 'AppMain'
}
</script>

<template>
    <div class="text-center mt-4 py-4">
        <img src="../assets/img-un/page-logo-1.png" alt="logo">
        <h3 class="mt-3">Inspirng by Excellence & Innovation</h3>
        <p>We offer a wide range of high quality of teaching and extra-curricular activities</p>
        <div class="mini-bar"></div>
    </div>
    <div class="ms-container">
        <div class="row g-0">
            <div class="col-8">
                <h2>Why Choose Avada University</h2>
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Labore delectus fuga eum quidem alias, nam iusto eius nisi possimus harum incidunt porro omnis, fugit dolorum enim cum laborum voluptatibus ipsa.
                Lorem ipsum dolor sit amet consectetur, adipisicing elit. Iure necessitatibus, asperiores, consequatur nostrum, placeat tenetur omnis ab totam quo molestiae porro harum sit reprehenderit. Error, id? Vel rem deserunt provident?</p>
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ex possimus iure sint tenetur veniam distinctio voluptate sapiente error! Nesciunt, non velit modi ipsa esse dignissimos voluptates eum at voluptas tempora.</p>
            </div>
            <div class="col-4 d-flex align-items-center justify-content-center ">
                <img class="" src="../assets/img-un/politics_seminar_event_feat-600x402.jpg" alt="#">
            </div>
        </div>

    </div>

    
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

.ms-container{
    img{
        width: 100%;
        height: 80%;
        object-fit: cover;
    }
}

</style>