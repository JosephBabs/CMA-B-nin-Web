<template>
  <div>
    <!--Site Footer One Start-->
    <footer class="site-footer">
      <div
        class="site-footer-bg"
        :style="`background-image: url(${require(`~/assets/images/backgrounds/footer-bg.jpg`)})`"
      ></div>
      <div class="container">
        <div class="site-footer__top">
          <div class="row">
            <div class="col-xl-3 col-lg-6 col-md-6">
              <div class="footer-widget__column footer-widget__about">
                <h3 class="footer-widget__title">Notre Mission</h3>
                <p class="footer-widget__text">
                  La Chambre Métiers de l'artisanat du Bénin a pour mission la représentation, la promotion du secteur et la protection des intérêts des artisans beninois et des entreprises artisanales auprès des collectivités locales, 
                  des instances nationales sous-régionales et internationales.
                </p>
                
              </div>
            </div>
            <div class="col-xl-3 col-lg-6 col-md-6">
              <div
                class="footer-widget__column footer-widget__explore clearfix"
              >
                <h3 class="footer-widget__title">Liens rapides</h3>
                <ul class="footer-widget__explore-list list-unstyled">
                  <li><nuxt-link to="/">Accueil</nuxt-link></li>
                  <li><nuxt-link to="/about">A propos</nuxt-link></li>
                  <li><nuxt-link to="/gallery">Gallerie</nuxt-link></li>
                  <li><nuxt-link to="/news">Actualités</nuxt-link></li>
                  <li><nuxt-link to="/contact">Contacts</nuxt-link></li>
                </ul>
                
              </div>
            </div>
            <div class="col-xl-3 col-lg-6 col-md-6">
              <div class="footer-widget__column footer-widget__contact">
                <h3 class="footer-widget__title">Contacts</h3>
                <ul class="list-unstyled footer-widget__contact-list">
                  <li>
                    <div class="icon">
                      <i class="icon-chat"></i>
                    </div>
                    <div class="text">
                      <p>
                        <span>Téléphone</span>
                        <a href="tel:+22940687884">+(229) 40 68 78 84</a>
                      </p>
                    </div>
                  </li>
                  <li>
                    <div class="icon">
                      <i class="icon-message"></i>
                    </div>
                    <div class="text">
                      <p>
                        <span>Adresse E-mail</span>
                        <a href="mailto:info@cmabenin.bj"
                          >info@cmabenin.bj</a
                        >
                      </p>
                    </div>
                  </li>
                  <li>
                    <div class="icon">
                      <i class="icon-address"></i>
                    </div>
                    <div class="text">
                      <p><span>Adresse</span>ZONE CEN-SAD/ Quartier Ahwanleko plage, a coté de la commission de l'UEMOA</p>
                    </div>
                  </li>
                </ul>
              </div>
            </div>
            <div class="col-xl-3 col-lg-6 col-md-6">
              <div class="footer-widget__column footer-widget__newsletter">
                <h3 class="footer-widget__title">Newsletter</h3>
                <p class="footer-widget__newsletter-text">
                  Inscrivez-vous à notre newsletter pour être informé de tout.
                </p>
                <form class="footer-widget__newsletter-form">
                  <input
                    type="email"
                    placeholder="E-mail"
                    name="email"
                  />
                  <button type="submit" class="footer-widget__newsletter-btn">
                    <i class="fas fa-arrow-circle-right"></i>Envoyer
                  </button>
                </form>
              </div>
            </div>
          </div>
        </div>
        <div class="site-footer__bottom">
          <div class="row">
            <div class="col-xl-12">
              <div class="site-footer__bottom-inner">
                <div class="site-footer__bottom-logo-social">
                  <div class="site-footer__bottom-logo">
                    <nuxt-link to="/">
                      <img
                        :src="require(`~/assets/images${logo.light}`)"
                        alt=""
                      />
                    </nuxt-link>
                  </div>
                  <!-- <div class="site-footer__bottom-social">
                    <a href="#"><i class="fab fa-twitter"></i></a>
                    <a href="#"><i class="fab fa-facebook-square"></i></a>
                    <a href="#"><i class="fab fa-dribbble"></i></a>
                    <a href="#"><i class="fab fa-instagram"></i></a>
                  </div> -->
                </div>
                <div class="site-footer__bottom-copy-right">
                  <p>&copy; Copyright {{ new Date().getFullYear() }} by <a href="#">Iroko-Media</a></p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </footer>
    <!--Site Footer One End-->
    <div v-if="sticky === true">
      <a
        @click="scrollTop"
        class="scroll-to-target scroll-to-top animated fadeInUp"
        ><i class="fa fa-angle-up"></i
      ></a>
    </div>
  </div>
</template>

<script>

const date = new Date().getFullYear();

import data from "~/data/data.json";
export default {
  data() {
    return {
      logo: data.logo,
      sticky: false,
    };
  },
  mounted() {
    window.addEventListener("scroll", this.handleScroll);
  },
  methods: {
    handleScroll() {
      if (window.scrollY > 70) {
        this.sticky = true;
      } else if (window.scrollY < 70) {
        this.sticky = false;
      }
    },
    scrollTop() {
      window.scrollTo(0, 0);
    },
  },
};
</script>
