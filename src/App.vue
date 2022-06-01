<template>
  <div id="app">
    <Nav></Nav> 
    <Header>
     
    </Header>
    <TheCanvas></TheCanvas>
    <About></About>
    <Portfolio></Portfolio>
    <WorkExperience></WorkExperience>
    <Educational></Educational>
    <Contact></Contact>
    <Footer></Footer>
  </div>
</template>

<script>
import Portfolio from "./components/Portfolio";
import Nav from "./components/Nav";
import Header from "./components/Header";
import About from "./components/About";
import WorkExperience from "./components/WorkExperience";
import Educational from "./components/Educational";
import Contact from "./components/Contact";
import Footer from "./components/footer";
import TheCanvas from './components/TheCanvas';

export default {
  name: "app",
  components: {
    Portfolio,
    Nav, 
    Header, 
    About,
    WorkExperience,
    Educational,
    Contact,
    Footer,TheCanvas
  }
};
</script>
<style>
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
body {
  font-family: Arial, Helvetica, sans-serif;
  line-height: 1.4;
}
</style>
