<template>
  <!-- Portfolio Grid -->
  <section class="bg-light page-section" id="portfolio">
    <div class="container">
      <div class="row">
        <div class="col-lg-12 text-center">
          <h2 class="section-heading text-uppercase">Portfolio</h2>
          <h3 class="section-subheading text-muted">
            Here are my portfolio since I have been work on web developer
          </h3>
        </div>
      </div>
      <div class="row">
        <div
          class="col-md-4 col-sm-6 portfolio-item"
          v-for="(obj, key) in portfolioJSON"
          :key="key"
        >
          <a class="portfolio-link" data-toggle="modal" :href="obj.href">
            <div class="portfolio-hover">
              <div class="portfolio-hover-content">
                <i class="fas fa-plus fa-3x"></i>
              </div>
            </div>
            <div class="portfolio-caption">
              <h4>{{ obj.caption }}</h4>
              <p class="text-muted">{{ obj.title }}</p>
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
        title: "React Project",
      },
      {
        img: "https://uppicimg.com/file/20IovSQX.jpg",
        caption: "PetCare",
        href: "https://taking-your-pet-with-pet-care.netlify.app/",
        title: "React Project",
      },
      {
        img:
          "https://content.codecademy.com/courses/intermediate-javascript-requests/wanderlust/background_photo_desktop.jpg",
        caption: "Wanderlust Check the WEATHER!",
        href: "https://wanderlust-weather.netlify.app/",
        title: "The WEATHER! - API HTTP Requests",
      },

      {
        img: "https://uppicimg.com/file/iE7L5gF6.jpg",
        caption: "Welcome to my Portfolio!",
        href: "",
        title: "VueJs Project",
      },

      {
        img:
          "https://scontent-atl3-2.xx.fbcdn.net/v/t1.6435-9/89053833_110699487202388_6827806855884963840_n.png?_nc_cat=100&ccb=1-5&_nc_sid=e3f864&_nc_ohc=OInd8x_5DpEAX_0t-yi&_nc_ht=scontent-atl3-2.xx&oh=00_AT90cjGwWX0W7ttzg6pF4Pp0AX8fjSEIJuNYlcloR3B4Cw&oe=61DE7FE0",
        caption: "iEnergywhiz",
        href: "https://www.ienergywhiz.com/",
        title: "React Project",
      },
      {
        img: "https://uppicimg.com/file/9gIqJSsY.jpg",
        caption: "Welcome to my World!",
        href: "https://welcome-to-myworld.netlify.app/",
        title: "Bootstrap Project",
      },
      {
        img: "https://uppicimg.com/file/5KARBkMN.jpg",
        caption: "NewsWeek",
        href: "https://news-week.netlify.app/",
        title: "Bootstrap ProjectNews",
      },
      {
        img: "https://uppicimg.com/file/0gUjFIcA.jpg",
        caption: "Portfolio - Dr. Norman Borlaug",
        href: "https://dr-norman-borlaug-page.netlify.app/",
        title: "HTML, CSS, Javascript Project",
      },

      {
        img:
          "https://chargerod.com/wp-content/uploads/2021/02/ptt-ev-charger.jpg",
        caption: "EV Station",
        href: "https://evstation.pttor.com/",
        title: "React/Redux Project",
      },
      {
        img: "https://miro.medium.com/max/1838/1*TlGoD3h0Dxawxx9k3AGO-g.png",
        caption: "killswitch.finance",
        href: "https://killswitch.finance/",
        title: "React Project Frontend",
      },
      {
        img:
          "https://marina-ferreira.github.io/img/tutorials/js/memory-game/memory-game.gif",
        caption: "Javascript Memory game",
        href: "https://js-memery-game.netlify.app/",
        title: "HTML, CSS, Javascript Project",
      },
    ],
  }),
};
</script>

<style slang="css"></style>
