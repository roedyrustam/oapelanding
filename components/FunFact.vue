<template>
  <section class="funfact-one" v-observe-visibility="onVisibilityChange">
    <div class="container">
      <div class="row">
        <div class="col-lg-3 col-md-6 col-sm-12 wow fadeInUp" data-wow-duration="1500ms" data-wow-delay="0ms">
          <div class="funfact-one__single">
            <h3 class="counter"> <countTo :startVal='0' :endVal='startCounter ? 7842 : 0' :duration='3000'></countTo></h3><!-- /.counter -->
            <p>Downloads</p>
          </div><!-- /.funfact-one__single -->
        </div><!-- /.col-lg-3 col-md-6 col-sm-12 -->
        <div class="col-lg-3 col-md-6 col-sm-12 wow fadeInUp" data-wow-duration="1500ms" data-wow-delay="100ms">
          <div class="funfact-one__single">
            <h3 class="counter"> <countTo :startVal='0' :endVal='startCounter ? 6020 : 0' :duration='3000'></countTo></h3><!-- /.counter -->
            <p>App Likes</p>
          </div><!-- /.funfact-one__single -->
        </div><!-- /.col-lg-3 col-md-6 col-sm-12 -->
        <div class="col-lg-3 col-md-6 col-sm-12 wow fadeInUp" data-wow-duration="1500ms" data-wow-delay="200ms">
          <div class="funfact-one__single">
            <h3 class="counter"> <countTo :startVal='0' :endVal='startCounter ? 360 : 0' :duration='3000'></countTo></h3><!-- /.counter -->
            <p>5 Star Rating</p>
          </div><!-- /.funfact-one__single -->
        </div><!-- /.col-lg-3 col-md-6 col-sm-12 -->
        <div class="col-lg-3 col-md-6 col-sm-12 wow fadeInUp" data-wow-duration="1500ms" data-wow-delay="300ms">
          <div class="funfact-one__single">
            <h3 class="counter"> <countTo :startVal='0' :endVal='startCounter ? 200 : 0' :duration='3000'></countTo></h3><!-- /.counter -->
            <p>Awards</p>
          </div><!-- /.funfact-one__single -->
        </div><!-- /.col-lg-3 col-md-6 col-sm-12 -->
      </div><!-- /.row -->
    </div><!-- /.container -->
  </section>
</template>

<script>
  import countTo from 'vue-count-to';
  import { ObserveVisibility } from 'vue-observe-visibility'

  export default {
    name: "FunFact",
    components: { countTo },
    directives: {
      ObserveVisibility
    },
    data() {
      return{
        startCounter: false
      }
    },
    methods: {
      onVisibilityChange (isVisible) {
        if (isVisible){
          this.startCounter = true;
        }

      },
    },
  }
</script>


<style scoped>

</style>
