<template>
  <!--Contact page Start-->
  <section class="contact-page">
    <div class="container">
      <div class="section-title text-center">
        <span class="section-title__tagline">Contactez-nous</span>
        <h2 class="section-title__title">
          Pour plus de renseignements <br />
          
        </h2>
      </div>
      <div class="row">
        <div class="col-xl-6 col-lg-6">
          <div class="contact-page__left">
            <div class="contact-page__img">
              <img src="~images/resources/contact-page-img-1.jpg" alt="" />
            </div>
            <p class="contact-page__text">
              La Chambre Métiers de l'artisanat du Bénin a pour mission la représentation, la promotion  du 
              secteur et la protection des intérêts des artisans beninois et des entreprises artisanales auprès 
              des collectivités locales, des instances nationales sous-régionales et internationales.
            </p>
            <div class="contact-page__contact-info">
              <ul class="contact-page__contact-list list-unstyled">
                <li>
                  <div class="icon">
                    <span class="icon-chat"></span>
                  </div>
                  <div class="text">
                    <p>Télémone</p>
                    <a href="tel:+22940687884">+(229) 40 68 78 84</a>
                  </div>
                </li>
                <li>
                  <div class="icon">
                    <span class="icon-message"></span>
                  </div>
                  <div class="text">
                    <p>Adresse E-mail</p>
                    <a href="mailto:info@cmabenin.bj"
                      >info@cmabenin.bj</a
                    >
                  </div>
                </li>
                <li>
                  <div class="icon">
                    <span class="icon-address"></span>
                  </div>
                  <div class="text">
                    <p>Adresse</p>
                    <h5>ZONE CEN-SAD/ Quartier Ahwanleko plage, a coté de la commission de l'UEMOA</h5>
                  </div>
                </li>
              </ul>
            </div>
          </div>
        </div>
        <div class="col-xl-6 col-lg-6">
          <div class="contact-page__form">
            <form
              action="#"
              class="contact-page__main-form contact-form-validated"
            >
              <div class="row">
                <div class="col-xl-12">
                  <div class="contact-page__input-box">
                    <input type="text" placeholder="Nom et prénom" name="name" />
                  </div>
                </div>
              </div>
              <div class="row">
                <div class="col-xl-6">
                  <div class="contact-page__input-box">
                    <input
                      type="email"
                      placeholder="Adresse E-mail"
                      name="email"
                    />
                  </div>
                </div>
                <div class="col-xl-6">
                  <div class="contact-page__input-box">
                    <input type="text" placeholder="Objet" name="subject" />
                  </div>
                </div>
              </div>
              <div class="row">
                <div class="col-xl-12">
                  <div class="contact-page__input-box">
                    <input
                      type="text"
                      placeholder="Numéro de téléphon ex: +229000000000"
                      name="phone"
                    />
                  </div>
                </div>
                <div class="col-xl-12">
                  <div class="contact-page__input-box">
                    <textarea
                      name="message"
                      placeholder="Saisissez votre message ici"
                    ></textarea>
                  </div>
                  <button type="submit" class="thm-btn contact-page__btn">
                    <i class="fas fa-arrow-circle-right"></i>Envoyer un message
                  </button>
                </div>
              </div>
            </form>
          </div>
        </div>
      </div>
    </div>
  </section>
  <!--Contact page End-->
</template>
