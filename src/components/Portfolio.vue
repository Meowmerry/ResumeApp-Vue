<template>
  <!-- Portfolio Grid -->
  <section class="bg-light page-section" id="portfolio">
    <div class="container">
      <div class="row">
        <div class="col-lg-12 text-center">
          <h2 class="section-heading text-uppercase">Portfolio</h2>
          <h3
            class="section-subheading text-muted"
          >Here are my portfolio since I have been work on web developer</h3>
        </div>
      </div>
      <div class="row">
        <div class="col-md-4 col-sm-6 portfolio-item" v-for="(obj,key) in portfolioJSON" :key="key">
          <a class="portfolio-link" data-toggle="modal" :href="obj.href">
            <div class="portfolio-hover">
              <div class="portfolio-hover-content">
                <i class="fas fa-plus fa-3x"></i>
              </div>
            </div>
            <div class="portfolio-caption">
              <h4>{{obj.caption}}</h4>
              <p class="text-muted">{{obj.title}}</p>
              <img class="img-fluid" v-bind:src="obj.img" alt />
            </div>
          </a>
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
        img: "https://uppicimg.com/file/BlDCJnMP.jpg",
        caption: "Restaurant Reservation",
        href: "https://restaurant-reservations-book.netlify.app/",
        title: "React Project"
      },
      {
        img: "https://uppicimg.com/file/20IovSQX.jpg",
        caption: "PetCare",
        href: "https://taking-your-pet-with-pet-care.netlify.app/",
        title: "React Project"
      },
      {
        img: "https://uppicimg.com/file/iE7L5gF6.jpg",
        caption: "Welcome to my World!",
         href: "",
        title: "VueJs Project"
      },
      {
        img: "https://uppicimg.com/file/5KARBkMN.jpg",
        caption: "NewsWeek",
         href: "https://news-week.netlify.app/",
        title: "Bootstrap ProjectNews"
      },
      {
        img: "https://uppicimg.com/file/0gUjFIcA.jpg",
        caption: "Portfolio - Dr. Norman Borlaug",
         href: "https://dr-norman-borlaug-page.netlify.app/",
        title: "HTML, CSS, Javascript Project"
      },
      {
         img: "https://uppicimg.com/file/9gIqJSsY.jpg",
        caption: "Welcome to my World!",
         href: "https://welcome-to-myworld.netlify.app/",
        title: "Bootstrap Project"
      }
    ]
  })
};
</script>

<style slang='css'>
</style>