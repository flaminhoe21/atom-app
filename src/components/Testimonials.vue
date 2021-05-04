<template>
    <div class="company-testimonials">
        <div class="section-intro">
            <div class="icon"><img src="@/assets/img/small-logo.png" alt="Small Company Logo"/></div>
            <h2>Vi anvendte HospiceGuiden fordi...</h2>
            <p>Consectetuer adpiscing praesent vestibulum lestie aenean nonummy hendrerit mauris phasellus suscipit varius mlorem
                ipsum dolor sit amet consectetue.</p>
        </div>
        <div class="customers-slider owl-carousel owl-theme" >
            <splide :options="options">
                <splide-slide  v-for="(obj, key) in testimonialsJSON" :key="key">
                    <div class="customer-shell">
                        <div class="profile-pic"><img :src="require(`@/assets/img/${obj.img}`)" alt="Profile Picture"/></div>
                        <div class="names">{{obj.name}}</div>
                        <div class="profession">{{obj.profession}}</div>
                    </div>
                </splide-slide>
            </splide>
        </div>
    </div>
</template>

<script>
    
   import { Splide, SplideSlide } from '@splidejs/vue-splide';
   import '@splidejs/splide/dist/css/themes/splide-default.min.css';


export default {
  components: {
    Splide,
    SplideSlide,

  },

   data() {
      return {
        options: {
          rewind : true,
          gap    : '1rem',
          autoplay: true,
          pagination: false,
        },
         testimonialsJSON: [
            {
                img: 'profile-pic.png',
                name: 'Karen Nielsem',
                profession: 'PHASELLUS SUWCIPIT VAIUS',
            },
            {
                img: 'profile-pic.png',
                name: 'Mark Dawson',
                profession: 'PROGRAMMER',
            },
            {
                img: 'profile-pic.png',
                name: 'Jason Lopez',
                profession: 'GRAPHIC DESIGNER',
            }
        ],
    };
  
;},

 
};
</script>

