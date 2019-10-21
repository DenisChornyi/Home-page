<template>
  <div id="app">
    <Menu />
    <Slider />
    <Section />
    <About />
    <Departments />
    <ClientsSay />
    <OurDoctors />
    <Contact />
    <Footer />
  </div>
</template>

<script>
import Menu from '../components/LayoutPartions/Menu.vue'
import Slider from '../components/home-page/Slider.vue'
import Section from '../components/home-page/SectionInfo.vue'
import About from '../components/home-page/About.vue'
import Departments from '../components/home-page/Departments.vue'
import ClientsSay from '../components/home-page/ClientsSay.vue'
import OurDoctors from '../components/home-page/OurDoctors.vue'
import Contact from '../components/home-page/Contact.vue'
import Footer from '../components/LayoutPartions/Footer.vue'
import 'bulma/css/bulma.css'
export default {
  name: 'app',
  components: {
    Menu,
    Slider,
    Section,
    About,
    Departments,
    ClientsSay,
    OurDoctors,
    Contact,
    Footer
  }
}
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css?family=Montserrat&display=swap');
  *{
    box-sizing: border-box;
    margin: 0;
    padding: 0;
  }
  h1{
    font-family: 'Montserrat', sans-serif;
    font-weight: 400;
  }
  h3{
    font-family: 'Montserrat', sans-serif;
    font-weight: 400;
    font-size: 20px;
  }
  h4{
    font-family: 'Montserrat', sans-serif;
    font-weight: 400;
  }
  p{
    color: #9b9b9b;
  }
</style>
