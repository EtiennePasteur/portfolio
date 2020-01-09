<template>
  <div>
    <div class="about">
      <div class="container d-flex flex-column">
        <div class="about-title">A little bit about myself.</div>
        <div class="about-desc d-flex flex-row justify-content-center align-items-center">
          <div class="circular-img">
            <img alt="me" class="img-memoji" src="~/assets/img/memoji.png" />
          </div>
          <div class="d-flex flex-column">
            <div>
              My name is Etienne Pasteur and I'm passionate about improving the lives of others through design. I'm constantly learning new things everyday and love meeting people who are motivated and unafraid of sharing their ideas with
              the world.
            </div>
            <div class="pt-4">
              I'm a self taught designer and have learnt a lot of the processes, concepts and theories of UX/UI and product design through attending workshops, reading blogs and applying these to projects in my spare time and at work. I am
              very much a big-picture thinker and enjoy working on products end to end, from ideation all the way to development.
            </div>
          </div>
        </div>
      </div>
      <div class="values background-yellow">
        <div class="container d-flex flex-column">
          <div class="d-flex flex-column">
            <div class="values-title">My values</div>
            <div class="values-item d-flex flex-column">
              <div class="values-item-title">😍 Passion is everything.</div>
              <div class="values-item-desc">
                If you don't enjoy what you're doing - move. You are not a tree. Channel your energy into something you believe in. I'm fortunate to be inspired and surrounded by motivated people who enjoy what they do. We only have so much
                time on this earth to live - so why waste it?
              </div>
            </div>
            <div class="values-item d-flex flex-column">
              <div class="values-item-title">🚀 Passion is everything.</div>
              <div class="values-item-desc">
                If you don't enjoy what you're doing - move. You are not a tree. Channel your energy into something you believe in. I'm fortunate to be inspired and surrounded by motivated people who enjoy what they do. We only have so much
                time on this earth to live - so why waste it?
              </div>
            </div>
            <div class="values-item d-flex flex-column">
              <div class="values-item-title">🏆 Passion is everything.</div>
              <div class="values-item-desc">
                If you don't enjoy what you're doing - move. You are not a tree. Channel your energy into something you believe in. I'm fortunate to be inspired and surrounded by motivated people who enjoy what they do. We only have so much
                time on this earth to live - so why waste it?
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="testimonials">
        <div class="container d-flex flex-column">
          <div class="d-flex flex-column">
            <div class="testimonials-title">Testimonials</div>
            <div class="testimonials-desc d-flex justify-content-center align-items-center">
              <b-carousel :interval="5000" class="testimonials-carousel" controls indicators>
                <b-carousel-slide img-blank>
                  <div class="testimonials-carousel-name">François Gonnet</div>
                  <div class="testimonials-carousel-company">UBG DIGITAL MEDIA</div>
                  <div class="testimonials-carousel-review">
                    Étienne est un excellent développeur full-stack. Sa pluridisciplinarité lui permet d’appréhender des projets IoT et Web complexes tout en étant force de proposition. Lead Developer sur de nombreux projets, il a gardé le
                    contrôle de chaque étape avec un grand professionnalisme.
                  </div>
                </b-carousel-slide>
                <b-carousel-slide img-blank>
                  <div class="testimonials-carousel-name">Kevin Labesse</div>
                  <div class="testimonials-carousel-company">NEO9</div>
                  <div class="testimonials-carousel-review">
                    Étienne est un bon développeur qui travaille vite et bien. Il est force de proposition et s'adapte rapidement au contexte des projets sur lesquels il travaille. Il a également un excellent relationnel avec ses clients.
                  </div>
                </b-carousel-slide>
                <b-carousel-slide img-blank>
                  <div class="testimonials-carousel-name">Malick Diagne</div>
                  <div class="testimonials-carousel-company">NEO9</div>
                  <div class="testimonials-carousel-review">
                    J'ai travaillé, sur plusieurs projets, avec Etienne et ce fut un réel plaisir. Il a un bon bagage technique et s'adapte rapidement aux différents défis qui se présente devant lui. Son intérêt pour la veille
                    technologique, sa pluridisciplinarité et sa détermination font de lui un bon élément. Je vous le recommande 👍
                  </div>
                </b-carousel-slide>
                <b-carousel-slide img-blank>
                  <div class="testimonials-carousel-name">Lionel Sgarbi</div>
                  <div class="testimonials-carousel-company">NEO9</div>
                  <div class="testimonials-carousel-review">
                    Très satisfait de ma collaboration avec Etienne. C'est un collaborateur sur qui on peut compter. Le code délivré est de qualité, les remontées d'alertes sont faites au bon moment et il sait moduler son investissement en
                    fonction des phases projet.
                  </div>
                </b-carousel-slide>
              </b-carousel>
            </div>
          </div>
        </div>
      </div>
      <div class="spacer"></div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
  .about {
    font-family: 'Avenir Next', sans-serif;
    padding-top: 20px;

    .spacer {
      margin-right: 100px;
      margin-left: 100px;
      border-style: solid;
      border-width: 0.5px;
      border-color: #ccc;
    }

    .background-yellow {
      background-color: #fff3ba;
    }

    .testimonials {
      margin: 60px 0;

      &-title {
        font-size: 36px;
        font-weight: 600;
      }

      &-carousel {
        width: 100%;
        height: 400px;

        &-name {
          font-weight: bold;
          font-size: 18px;
        }

        &-company {
          padding-bottom: 15px;
          font-weight: 600;
        }

        &-review {
          font-style: italic;
        }

        @media (min-width: 576px) {
          height: 300px;
        }
      }
    }

    .values {
      margin-top: 60px;
      padding: 20px 0 30px;

      &-title {
        font-size: 36px;
        font-weight: 600;
        padding-top: 30px;
      }

      &-item {
        padding: 30px 0;

        &-title {
          font-size: 26px;
          font-weight: 600;
        }

        &-desc {
          font-size: 16px;
        }
      }
    }

    @media (min-width: 576px) {
      padding-top: 40px;
    }

    @media (min-width: 768px) {
      padding-top: 60px;
    }

    &-title {
      font-size: 40px;
      font-weight: 600;
    }

    &-desc {
      margin: 55px 0 30px;
    }

    .circular-img {
      display: none;
      justify-content: center;
      align-items: center;
      border-radius: 50%;
      background: #99cbfa;
      height: 140px;
      width: 140px;
      min-width: 140px;
      margin: 0 30px 0 15px;

      @media (min-width: 768px) {
        display: flex;
      }
    }

    .circular-img img {
      width: 100%;
      height: 100%;
      margin: 12px 0 0 20px;
    }
  }
</style>
