<template>
  <div id="title" class="d-flex justify-content-center m-3 p-1 rounded-lg">
    <img src="~assets/zach.png" class="img-fluid mr-3" />
    <h1 class="display-3 my-auto">Zach Jokes</h1>
    <img src="~assets/zach.png" class="img-fluid ml-3" />
  </div>
</template>

<style scoped>
img {
    max-width: 8rem;
}
@media (max-width:375px) {
    img {
        display: none;
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