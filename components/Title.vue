<template>
<div id="title" class="m-3 p-1 rounded-lg">
  <img id="img-sm" src="~assets/zach.png" class="img-fluid">
  <span  class="d-flex justify-content-center">
    <img id="img1" src="~assets/zach.png" class="img-fluid mr-3">
    <h1 class="display-3 my-auto">Zach Jokes</h1>
    <img id="img2" src="~assets/zach.png" class="img-fluid ml-3">
  </span>
</div>
</template>

<style scoped>
img {
    max-width: 8rem;
}
#img-sm {
    display: none;
    height: 15vh;
    margin-top: 0.5rem;
    margin-left: auto;
    margin-right: auto;
}
@media (max-width:375px) {
    #img1, #img2 {
        display: none;
    }
    #img-sm {
        display: block;
    }
    h1 {
        padding-top: 1rem;
        padding-bottom: 1rem;
        font-size: 45px;
        width: 100%;
    }
}
h1 {
  color: #ffffff;
  vertical-align: middle;
  text-align: center;
  font-weight: 400;
}
#title {
    background: rgba(255, 255, 255, 0.1);
}
</style>