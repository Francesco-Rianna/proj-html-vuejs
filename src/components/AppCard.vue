<script>
export default {
    name : 'AppCard'
}
</script>

<template>
    <div class="ms-container">
            <div class="row ">
                <div class="col-4">
                    <div class="card">
                       <img src="../assets/img-un/news_single_post_header_1-600x333.jpg" class="card-img-top" alt="...">
                       <div class="card-body p-3">
                          <div class="card-text color-orange"> What do succesful grads think you should study?</div>
                          <div class="text-small mt-1"> By <a href="" class="color-orange">admin </a>| <span> March 16th,2016</span></div>
                          <div class="mt-3 d-flex justify-content-between color-orange text-small">
                            <div>Read More</div>
                            <div>
                                <i class="fa-regular fa-comment me-2"></i>
                                <span>0</span>
                            </div>
                          </div>
                       </div>
                    </div>
                </div>
                <div class="col-4">
                    <div class="card">
                       <img src="../assets/img-un/news_single_post_header_2-800x444.jpg" class="card-img-top" alt="...">
                       <div class="card-body p-3">
                          <div class="card-text color-orange"> What do succesful grads think you should study?</div>
                          <div class="text-small mt-1"> By <a href="" class="color-orange">admin </a>| <span> March 16th,2016</span></div>
                          <div class="mt-3 d-flex justify-content-between color-orange text-small">
                            <div>Read More</div>
                            <div> 
                                <i class="fa-regular fa-comment me-2"></i>
                                <span>0</span>
                            </div>
                          </div>
                       </div>
                    </div>
                </div>
                <div class="col-4">
                    <div class="card">
                       <img src="../assets/img-un/news_single_post_header_3.jpg" class="card-img-top" alt="...">
                       <div class="card-body p-3">
                          <div class="card-text color-orange"> What do succesful grads think you should study?</div>
                          <div class="text-small mt-1"> By <a href="" class="color-orange">admin </a>| <span> March 16th,2016</span></div>
                          <div class="mt-3 d-flex justify-content-between color-orange text-small">
                            <div>Read More</div>
                            <div>
                                <i class="fa-regular fa-comment me-2"></i>
                                <span>0</span>
                            </div>
                          </div>
                       </div>
                    </div>
                </div>
                
            </div>


                
              
            
    </div>
</template>

<style scoped lang="scss">
 @use '../style/variables' as *;
.ms-container{
    img{
        width: 100%;
        height: 80%;
        object-fit: cover;
    }
}

.color-orange{
    color : $color-orange;
    font-weight: bold;

}

.text-small{
    font-size: 12px;
}


</style>