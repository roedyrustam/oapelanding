<template>
  <div>
    <footer class="site-footer">
      <div class="site-footer__upper">
        <div class="container">
          <div class="row">
            <div class="col-xl-4 col-lg-6">
              <div class="footer-widget footer-widget__about">
                <a href="/" class="logo">
                  <img src="/assets/images/logo-1-2.png" width="136" alt="" />
                </a>
                <p>
                  Lorem Ipsum is simply dummy text the <br />
                  printing and setting industry. Lorm Ipsum <br />
                  has been the text ever.
                </p>
                <a href="#" class="thm-btn"><span>Download App</span></a
                ><!-- /.thm-btn -->
              </div>
              <!-- /.footer-widget footer-widget__about -->
            </div>
            <!-- /.col-lg-4 -->
            <div class="col-xl-2 col-lg-6">
              <div class="footer-widget footer-widget__links">
                <h3 class="footer-widget__title">Explore</h3>
                <!-- /.footer-widget__title -->
                <ul class="list-unstyled footer-widget__links-list">
                  <li><a href="#">About</a></li>
                  <li><a href="#">Our Team</a></li>
                  <li><a href="#">Contact</a></li>
                  <li><a href="#">Services</a></li>
                </ul>
                <!-- /.list-unstyled footer-widget__links-list -->
              </div>
              <!-- /.footer-widget footer-widget__links -->
            </div>
            <!-- /.col-lg-2 -->
            <div class="col-xl-2 col-lg-6">
              <div class="footer-widget footer-widget__contact">
                <h3 class="footer-widget__title">Contact</h3>
                <!-- /.footer-widget__title -->
                <ul class="footer-widget__contact-list list-unstyled">
                  <li>
                    <i class="fa fa-phone-square"></i>
                    <a href="tel:777-888-0000">777 888 0000</a>
                  </li>
                  <li>
                    <i class="fa fa-envelope"></i>
                    <a href="mailto:needhelp@oapee.com">needhelp@oapee.com</a>
                  </li>
                  <li>
                    <i class="fa fa-map-marker"></i>
                    855 road, broklyn street <br />
                    new york 600
                  </li>
                </ul>
                <!-- /.footer-widget__contact-list list-unstyled -->
              </div>
              <!-- /.footer-widget footer-widget__contact -->
            </div>
            <!-- /.col-lg-2 -->
            <div class="col-xl-4 col-lg-6">
              <div class="footer-widget footer-widget__newsletter">
                <h3 class="footer-widget__title">Newsletter</h3>
                <form action="#" class="footer-widget__newsletter-form">
                  <input type="text" placeholder="Email address" name="email" />
                  <button type="submit"><i class="fa fa-envelope"></i></button>
                </form>
                <!-- /.footer-widget__newsletter-form -->
                <p>
                  Sign up for our latest news & articles. We won’t give you spam
                  mails.
                </p>
              </div>
              <!-- /.footer-widget footer-widget__newsletter -->
            </div>
            <!-- /.col-lg-4 -->
          </div>
          <!-- /.row -->
        </div>
        <!-- /.container -->
      </div>
      <!-- /.site-footer__upper -->
      <div class="site-footer__bottom">
        <div class="container">
          <div class="inner-container">
            <p>© copyright 2022 Pandu Talenta Digital</p>
            <div class="footer-social">
              <a href="#"><i class="fab fa-facebook-square"></i></a>
              <a href="#"><i class="fab fa-twitter"></i></a>
              <a href="#"><i class="fab fa-instagram"></i></a>
              <a href="#"><i class="fab fa-pinterest-p"></i></a>
            </div>
            <!-- /.footer-social -->
          </div>
          <!-- /.inner-container -->
        </div>
        <!-- /.container -->
      </div>
      <!-- /.site-footer__bottom -->
    </footer>

    <a
      @click="scrollTop"
      class="scroll-to-target scroll-to-top"
      :style="`display: ${scrollBtn ? 'inline' : 'none'}`"
      href="#"
      ><i class="fa fa-angle-up"></i
    ></a>
  </div>
</template>

<script>
export default {
  name: "Footer",
  data() {
    return {
      scrollBtn: false
    };
  },
  mounted() {
    window.addEventListener("scroll", this.handleScroll);
  },

  methods: {
    handleScroll() {
      if (window.scrollY > 70) {
        this.scrollBtn = true;
      } else if (window.scrollY < 70) {
        this.scrollBtn = false;
      }
    },

    scrollTop() {
      window.scrollTo(0, 0);
    }
  }
};
</script>

<style scoped></style>
