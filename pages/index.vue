<template>
  <div>
    <Nav />
    <Banner />
    <Service />
    <CallToActionFour />
    <Brands />
    <CallToActionThree />
    <CallToActionTwo />
    <Video />
    <Pricing />
    <Testimonial />
    <FunFact />
    <Screenshots />
    <Faq />
    <BlogArea />
    <CallToAction />
    <Footer />
  </div>
</template>

<script>

  import Nav from "../components/Nav";
  import Banner from "../components/Banner";
  import Service from "../components/Service";
  import CallToActionFour from "../components/CallToActionFour";
  import Brands from "../components/Brands";
  import CallToActionThree from "../components/CallToActionThree";
  import CallToActionTwo from "../components/CallToActionTwo";
  import Video from "../components/Video";
  import Pricing from "../components/Pricing";
  import Testimonial from "../components/Testimonial";
  import Screenshots from "../components/Screenshots";
  import FunFact from "../components/FunFact";
  import Faq from "../components/Faq";
  import BlogArea from "../components/BlogArea";
  import CallToAction from "../components/CallToAction";
  import Footer from "../components/Footer";
  export default {
    components: {
      Footer,
      CallToAction,
      BlogArea,
      Faq,
      FunFact,
      Screenshots,
      Testimonial,
      Pricing,
      Video,
      CallToActionTwo,
      CallToActionThree,
      Brands,
      CallToActionFour,
      Service,
      Banner,
      Nav

    }
  }
</script>
