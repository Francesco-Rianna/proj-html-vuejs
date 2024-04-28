<template>
  <div class="hero d-flex justify-content-center align-items-center">
    <div class="content text-center">
      <h1>Inspirng tommorow leaders</h1>
      <h3 class="my-3 ">The future Belongs To Those Who See Possibilities Today</h3>
      <div class="mt-4">
        <button class="mx-2 bg-orange py-2 px-3"> <a href=""> FIND A COURSE</a></button>
        <button class="py-2 px-3 bg-sky"> <a href="">APPLY NOW</a></button>
      </div>
    </div>
  </div>
</template>


<style scoped lang="scss">
@use '../style/variables' as *;
.hero {
  background-image: url('../assets/img-un/home_main_slider_bg.jpg');
  background-position: bottom;
  background-size: cover;
  height: 600px;
}

.content {
  color: $color-white;
  h1 {
    font-size: 80px;
  }
}
button{
  color: $color-white;
}

.bg-orange {
  background-color: $color-orange;
}

.bg-sky{
  background-color: $color-sky;
}
</style>