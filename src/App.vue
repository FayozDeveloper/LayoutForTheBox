<template>
  <div>
        <TestNavbar/>
<!--        <Navbar/>-->
        <div class='Hero'>
          <MainPage/>
        </div>
        <Reasons/>
        <About/>
        <Services/>
        <Stats_/>
        <Ads_/>
    <ProjectsPage/>
    <Fom_/>
    <Bottom_section/>
    <Footer_section/>
  </div>
</template>

<script>
// import Navbar from "@/components/Navbar";
import MainPage from "@/components/MainPage";
import Reasons from "@/components/Reasons";
import About from "@/components/About";
import Services from "@/components/Services";
import Stats_ from "@/components/Stats";
import Ads_ from "@/components/Ads";
import ProjectsPage from "@/components/ProjectsPage";
import Fom_ from "@/components/Fom";
import Footer_section from "@/components/Footer";
import Bottom_section from "@/components/Bottom";
import TestNavbar from "@/components/TestNavbar";


export default {
  name: 'App',
  components: {
    TestNavbar,
    Bottom_section,
    Footer_section,
    Fom_,
    ProjectsPage,
    Ads_,
    Stats_,
    Services,
    About,
    Reasons,
    MainPage,
    // Navbar,
  }
}

</script>

<style>
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
.Hero{
  width: 100%;
  height: 646px;
  background-image: url("./assets/Heroimg.jpg");
  background-repeat: no-repeat;
  background-size: cover;
}
#app{
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}

</style>
