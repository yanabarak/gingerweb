<template>
  <section class="align-self-start col-12 section-book" id="proportions-book">
    <div class="content">
      <h1 class="mb-4">Logo & Icon Proportions</h1>
      <p class="mb-50">
        The Guberman Logo has a neat proportion of 4:1 width.<br />
        These proportions were chosen carefully and they are not to be changed.<br />
        The Icon has a perfect square proportion of 1:1 and acts as the Favicon as well.
      </p>
      <div class="proportions-1 mb-50 ms-md-5">
        <img src="../assets/proportions.png" alt="proportions 1" />
      </div>
      <div class="proportions-2 mb-50 mx-auto">
        <img src="../assets/proportions2.png" alt="proportions 2" />
      </div>
    </div>
  </section>
</template>
<style scoped>
#proportions-book {
  padding-top: 150px;
  min-height: 120vh;
}
.proportions-1 {
  width: 454px;
  height: 200px;
}
.proportions-2 {
  width: 120px;
  height: 120px;
}
.proportions-1 img,
.proportions-2 img {
  width: 100%;
  height: 100%;
  object-fit: contain;
}

@media screen and (max-width: 1200px) {
  #proportions-book {
    min-height: unset;
  }
}

@media screen and (max-width: 992px) {
  #proportions-book {
    padding-top: 100px;
  }

  .proportions-1 {
    max-width: 100%;
    max-height: 200px;
  }
}
</style>
