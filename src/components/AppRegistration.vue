<script>
export default {
    name : 'AppRegistration'
}
</script>

<template>
    <div class="bg-registration py-5">
        <div class="text-center">
           <div> Joing Over <span class="underline">500.000 Students</span> Enjoyng Avada Education Now </div> 
            <div class=" small">Become Part Of Avada University to Further Your Career</div>
        </div>
        <div class="ms-container mt-5">
            <div class="d-flex justify-content-around">
                <input class="py-2 px-3" placeholder="Name">
                <input class="py-2 px-3" placeholder="Email">
                <input class="py-2 px-3" placeholder="Telephone">
                <button>APPLY NOW</button>
            </div>
        </div>
    </div>
</template>
        
        


<style scoped lang="scss">
@use '../style/variables' as *;
.bg-registration{
    background-color: $color-gray-d;
}

.text-center{
    font-size: 25px;
    color: $color-white;
    span{
        color : $color-orange
    }
    .small{
        font-size: 15px;
        color : $color-gray
    }
}

.underline {
    position: relative;
    display: inline-block;
}

.underline::after {
    content: '';
    position: absolute;
    bottom:0; 
    left: 0;
    width: 100%;
    height: 2px; 
    background-color: $color-orange; 
    border-radius: 30px; 
}

input{
    background: #444d63;
    border: none;
    width: 25%;
   
}
input::placeholder{
    color : $color-white
}

button{
    width: 18%;
    background: $color-orange;
    color: $color-white;
    font-weight: bold;
}
</style>