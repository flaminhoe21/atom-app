<template>
    <Header></Header>
        <div id="slider">
            <div class="slider-wrap">
                <div class="images-holder">
                    <ul>
                    <splide :options="options">
                        <splide-slide><li><img src="./assets/img/slider-image.jpg" alt="Silder Image"/></li></splide-slide>
                        <splide-slide><li><img src="./assets/img/slider-image-1.jpg" alt="Silder Image 2"/></li></splide-slide>
                        <splide-slide><li><img src="./assets/img/slider-image-2.jpg" alt="Silder Image 3"/></li></splide-slide>
                    </splide>
                    </ul>
                    <div class="text-holder">
                    <div class="wrapper">
                        <h1>Nemo voluptatem quia voluptas </h1>
                        <h2>dolores ratione voluptatem</h2>
                    </div>
                </div>
            </div>
        </div>
        <div class="slider-underline">
            <p>Når den sidste tid skal elskes...</p>
        </div>
      </div>

      <div id="app">
          <div class="wrapper">
              <div class="about-company">
                  <div class="intro-text">
                      <p>Consecteur adipisicin in elusmos tempor incididunt the labore dolore is magnaliua veniam nostrud exercitation in ullamco
                          laboris aliquip an consequa the prehene  occaecas cupidatat laborum erspiciatis unomnis voluptatem there accusantium laudantium aperiam.</p>
                  </div>
                  <dov class="read-more-btn"><a href="#">Read More</a></dov>
                  <div class="grid-structure">
                      <div class="single-grid left">
                          <div class="row full-image top">
                              <div class="cell">
                                  <a href="#">
                                      <div class="image-holder"><img src="./assets/img/windows.jpg" alt="Windows Image"/></div>
                                      <span>UDVALGT HOSPICE LÆS OM DERES TRYGHEDSCERTIFIKAT</span>
                                  </a>
                              </div>
                          </div>
                          <div class="row two-sided">
                              <div class="cell left">
                                  <a href="#">
                                      <div class="image-holder"><img src="./assets/img/elder-people.jpg" alt="Elder People"/></div>
                                      <span>Mauris maximus nisi et sapien tristique, quis </span>
                                  </a>
                              </div>
                              <div class="cell right">
                                  <a href="#">
                                      <div class="image-holder"><img src="./assets/img/office-atm.jpg" alt="Office Atm"/></div>
                                      <span>Aenean suscipit leo nec est convallis faucibus</span>
                                  </a>
                              </div>
                          </div>
                      </div>
                      <div class="single-grid right">
                          <div class="row two-sided">
                              <div class="cell company-banner left">
                                  <a href="#">
                                      <div class="image-holder"><img src="./assets/img/grey-background.jpg" alt="Grey Background"/></div>
                                      <div class="banner-info">
                                          <div class="logo"><img src="./assets/img/hops-banner-logo.png" alt="Company Logo"/></div>
                                          <span>HVILKET HOSPICE ER BEDST</span>
                                          <a href="#" class="read-more-btn">Read More</a>
                                          
                                          
                                      </div>
                                  </a>
                              </div>
                              <div class="cell right">
                                  <a href="#">
                                      <div class="image-holder"><img src="./assets/img/support.jpg" alt="Support Image"/></div>
                                      <span>Lorem ipsum dolor sit amet, consectetur</span>
                                  </a>
                              </div>
                          </div>
                          <div class="row full-image bottom">
                              <div class="cell">
                                  <a href="#">
                                      <div class="image-holder"><img src="./assets/img/project-img.jpg" alt="Project Image"/></div>
                                      <span>HVAD KAN VI FORVENTE I FREMTIDEN</span>
                                  </a>
                              </div>
                          </div>
                      </div>
                  </div>
              </div>

              <div class="company-pros">
                  <div class="section-intro">
                      <h2>HOSPICEGUIDEN</h2>
                      <p>Lorem ipsum dolor sit amet, potenti at torquent dui augue nunc mattis an vulputate totam curabitur ante imperdiet
                          vestibulum sem pede ut dolor sem in sem suspendisse nec duis, nibh sit laoreet eu vitae enim odio id mollis fusce est tempor.</p>
                  </div>
                  <div class="box-elements">
                      <div class="single-box">
                          <div class="icon-holder"><img src="./assets/img/phone-icon.png" alt="Phone Icon"/></div>
                          <span>KONTAKT HOSPICEGUIDEN</span>
                      </div>
                      <div class="single-box">
                          <div class="icon-holder"><img src="./assets/img/earth-icon.png" alt="Earth Icon"/></div>
                          <span>FIND DET NÆRMESTE HOSPICE</span>
                      </div>
                      <div class="single-box">
                          <div class="icon-holder"><img src="./assets/img/percent-icon.png" alt="Percent Icon"/></div>
                          <span>KONTAKT HOSPICEGUIDEN</span>
                      </div>
                  </div>
              </div>

              <Testimonials></Testimonials>
          </div>
      </div>
    <Footer></Footer>
  

    
</template>


<script>
    
import { Splide, SplideSlide } from '@splidejs/vue-splide';
import '@splidejs/splide/dist/css/themes/splide-default.min.css';
import Testimonials from './components/Testimonials.vue';
import Header from './components/Header.vue';
import Footer from './components/Footer.vue';

export default {
  name: "app",
  components: {
    Splide,
    SplideSlide,
    Testimonials,
    Header,
    Footer
  },
  data() {
      return {
        options: {
          rewind : true,
          gap    : '1rem',
          autoplay: true,
          pagination: false,
        },
    };},
  
    
 
};
</script>


<style>
@font-face {
	font-family: 'Montserrat';
	font-style: normal;
	font-weight: 300;
	font-display: swap;
	src: url(https://fonts.gstatic.com/s/montserrat/v15/JTURjIg1_i6t8kCHKm45_cJD3gnD_g.woff2) format('woff2');
	unicode-range: U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+2000-206F, U+2074, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;
}

/* latin */
@font-face {
	font-family: 'Montserrat';
	font-style: normal;
	font-weight: 500;
	font-display: swap;
	src: url(https://fonts.gstatic.com/s/montserrat/v15/JTURjIg1_i6t8kCHKm45_ZpC3gnD_g.woff2) format('woff2');
	unicode-range: U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+2000-206F, U+2074, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;
}
/* latin */
@font-face {
	font-family: 'Montserrat';
	font-style: normal;
	font-weight: 600;
	src: url(https://fonts.gstatic.com/s/montserrat/v15/JTURjIg1_i6t8kCHKm45_bZF3gnD_g.woff2) format('woff2');
	unicode-range: U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+2000-206F, U+2074, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;
}

  /* latin */
@font-face {
	font-family: 'Montserrat';
	font-style: normal;
	font-weight: 700;
	font-display: swap;
	src: url(https://fonts.gstatic.com/s/montserrat/v15/JTURjIg1_i6t8kCHKm45_dJE3gnD_g.woff2) format('woff2');
	unicode-range: U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+2000-206F, U+2074, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;
}
</style>