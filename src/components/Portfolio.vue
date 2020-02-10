<template>
  <!-- Portfolio Grid -->
  <section class="bg-light page-section" id="portfolio">
    <div class="container">
      <div class="row">
        <div class="col-lg-12 text-center">
          <h2 class="section-heading text-uppercase">Portfolio</h2>
          <h3 class="section-subheading text-muted">Here are my portfolio since I have been work on web developer</h3>
        </div>
      </div>
      <div class="row">
        <div class="col-md-4 col-sm-6 portfolio-item" v-for="(obj,key) in portfolioJSON" :key="key">
          <a class="portfolio-link" data-toggle="modal" href="#portfolioModal1">
            <div class="portfolio-hover">
              <div class="portfolio-hover-content">
                <i class="fas fa-plus fa-3x"></i>
              </div>
            </div>
            <img class="img-fluid" src="img" alt />
          </a>
          <div class="portfolio-caption">
            <h4>{{obj.caption}}</h4>
            <p class="text-muted">{{obj.title}}</p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
<script>
export default {
  data: () => ({
    portfolioJSON: [
      {
        img: "https://uppicimg.com/file/WJd1DLnB.jpg",
        caption: "Restaurant Reservation",
        title: "React Project"
      },
      {
        img: "https://uppicimg.com/file/WJd1DLnB.jpg",
        caption: "PetCare",
        title: "React Project"
      },
      {
        img: "https://uppicimg.com/file/WJd1DLnB.jpg",
        caption: "Welcome to my World!",
        title: "Bootstrap Project"
      },
      {
        img: "https://uppicimg.com/file/WJd1DLnB.jpg",
        caption: "NewsWeek",
        title: "Bootstrap ProjectNews"
      },
      {
        img: "https://uppicimg.com/file/WJd1DLnB.jpg",
        caption: "Portfolio - Dr. Norman Borlaug",
        title: "HTML, CSS, Javascript Project"
      },
      {
        img: "https://uppicimg.com/file/WJd1DLnB.jpg",
        caption: "My Resume",
        title: "HTML, CSS, Javascript Project"
      }
    ]
  })
};
</script>

<style slang='css'>
</style>