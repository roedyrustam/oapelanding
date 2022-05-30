<template>
  <section class="banner-one" id="home">
    <img
      src="/assets/images/shapes/banner-shape-1-1.png"
      class="banner-one__bg-shape-1"
      alt=""
    />
    <img
      src="/assets/images/shapes/banner-shape-1-2.png"
      class="banner-one__bg-shape-2"
      alt=""
    />
    <img
      src="/assets/images/shapes/banner-shape-1-3.png"
      class="banner-one__bg-shape-3"
      alt=""
    />
    <img
      src="/assets/images/shapes/banner-shape-1-4.png"
      class="banner-one__bg-shape-4"
      alt=""
    />
    <img
      src="/assets/images/shapes/banner-shape-1-5.png"
      class="banner-one__bg-shape-5"
      alt=""
    />

    <div class="container">
      <div class="row">
        <div class="col-lg-6 d-flex">
          <div class="my-auto">
            <div class="banner-one__content">
              <h3>
                Manage Project <br />
                With The Best <br />
                Application
              </h3>
              <p>Dengan Singele Page Component <br />Lebih Cepat dan efisien</p>
              <a href="#" class="thm-btn banner-one__btn"
                ><span>Discover More</span></a
              >
              <!-- /.thm-btn banner-one__btn -->
            </div>
            <!-- /.banner-one__content -->
          </div>
          <!-- /.my-auto -->
        </div>
        <!-- /.col-lg-6 -->
        <div
          class="col-lg-6 d-flex justify-content-end wow fadeInUp"
          data-wow-duration="1500ms"
        >
          <div class="banner-one__image">
            <img src="/assets/images/resources/banner-1-moc-1.png" alt="" />
          </div>
          <!-- /.banner-one__image -->
        </div>
        <!-- /.col-lg-6 -->
      </div>
      <!-- /.row -->
    </div>
    <!-- /.container -->
  </section>
</template>

<script>
export default {
  name: "Banner"
};
</script>

<style scoped></style>
