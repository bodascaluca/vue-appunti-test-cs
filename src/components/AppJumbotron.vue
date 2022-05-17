<template>
  <div>
    <div class="jumbotron-img">
      <h1>{{ titleText }}</h1>
      <img
        class="jumbotron-container-img"
        src="../assets/img/footer-bg.jpg"
        alt=""
      />
      <h3 class="title active">Salve</h3>
    </div>
  </div>
</template>

<script>
export default {
  name: "AppJumbotron",
  data: function () {
    return {
      titleText: `Ciao mondo`,
    };
  },
};
</script>

<style scoped lang="scss">
@import "../style/variable.scss";
.jumbotron-img {
  position: relative;
  width: 100%;
  height: 300px;
  //   background-image: url("../assets/img/footer-periscope.png");

  h3 {
    &.img {
      filter: grayscale(1);
    }
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    color: white;
    text-decoration: uppercase;
    font-size: 2rem;

    &.active {
      background-color: red;
    }

    &:hover {
      color: green;
    }
  }
}

img {
  max-width: 50%;
}
</style>
