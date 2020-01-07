<template>
  <div class="container">
    <div class="presentation d-flex flex-column">
      <div class="presentation-bold presentation-name">
        Hi, I'm
        <span class="text-yellow text-white-shadow-hover">Etienne Pasteur</span>
      </div>
      <div class="presentation-bold presentation-jobs">
        <client-only>
          I do awesome stuff like
          <vue-typer
            :text="stuff"
            :repeat="Infinity"
            :shuffle="true"
            :pre-type-delay="100"
            :type-delay="120"
            :pre-erase-delay="1600"
            :erase-delay="75"
            :erase-on-complete="false"
            initial-action="typing"
            erase-style="backspace"
            caret-animation="blink"
            class="text-white-shadow text-green"
          />
        </client-only>
      </div>
      <div class="presentation-desc">
        <div class="presentation-desc-title">I am a 23 years old Full-Stack JavaScript Developer based in Lyon - France 🥖🇫🇷</div>
        <div class="presentation-desc-desc">
          I have experience in delivering scalable web applications with trending frameworks such as Angular, Vue or React. I'm passionate about coding, DevOps, UI/UX & many more related fields. I am also constantly looking to learn new
          things everyday.
        </div>
      </div>
    </div>
    <div class="work d-flex flex-column mb-5">
      <div class="work-title mb-5">MY RECENT WORK</div>
      <div class="work-item work-item-blue">
        <div v-aspect-ratio="'16:6'">
          <div class="work-item-container overflow-hidden">
            <div class="d-flex flex-row align-items-center justify-content-center w-100 h-100">
              <img class="img-neo9" src="~/assets/img/Neo9.png" alt="neo9" />
              <div class="d-flex flex-column">
                <div class="work-item-title">AprilOn</div>
                <div class="work-item-desc">Building a marketplace for insurance</div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="work-item work-item-yellow">
        <div v-aspect-ratio="'16:6'">
          <div class="work-item-container overflow-hidden">
            <div class="d-flex flex-row align-items-center justify-content-center w-100 h-100">
              <div class="d-flex flex-column mr-4">
                <div class="work-item-title">iBubble</div>
                <div class="work-item-desc">Prototyping the first autonomous diving drone</div>
              </div>
              <img class="img-sogilis" src="~/assets/img/Sogilis.png" alt="sogilis" />
            </div>
          </div>
        </div>
      </div>
      <div class="work-item work-item-green">
        <div v-aspect-ratio="'16:6'">
          <div class="work-item-container overflow-hidden">
            <div class="d-flex flex-row align-items-center justify-content-center w-100 h-100">
              <img class="img-ubg" src="~/assets/img/Ubg.png" alt="ubg" />
              <div class="d-flex flex-column">
                <div class="work-item-title">Meet Your Beauty</div>
                <div class="work-item-desc">Integrating a website dedicated to beauty</div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        stuff: ['coding', 'building drones', 'flying', 'traveling', 'listening to music', 'taking photos']
      }
    }
  }
</script>
<style lang="scss">
  .work {
    font-family: 'Avenir Next', sans-serif;

    &-title {
      color: #757678;
      font-size: 14px;
      line-height: 24px;
      font-weight: 400;
      letter-spacing: 1px;
      text-transform: uppercase;
    }

    &-item {
      color: #191b1e;
      font-weight: normal;
      letter-spacing: 0;
      margin: 10px 0;
      border-radius: 3px;
      box-shadow: 0 2px 4px 0 rgba(0, 0, 0, 0.08);
      position: relative;
      cursor: pointer;

      &:hover {
        box-shadow: 0 2px 4px 0 rgba(0, 0, 0, 0.2);
        transform: scale(1.01);
        transition: opacity 1000ms ease, transform 450ms ease, -webkit-transform 450ms ease;
      }

      &-title {
        font-family: 'Geller Headline', sans-serif;
        font-weight: 600;
        font-size: 3vw;
        line-height: 3.5vw;
        letter-spacing: 0.4px;
      }

      &-desc {
        font-size: 1.6vw;
      }

      .img {
        &-neo9 {
          height: 65%;
          position: relative;
          left: -15%;
        }

        &-ubg {
          height: 65%;
          position: relative;
          left: -15%;
        }

        &-sogilis {
          height: 65%;
          position: relative;
          right: -4%;
        }
      }

      &-container {
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
      }

      &-blue {
        background-color: #99cbfa;
      }

      &-green {
        background-color: #9ee8d1;
      }

      &-yellow {
        background-color: #ffe993;
      }
    }
  }

  .presentation {
    font-family: 'Avenir Next', sans-serif;
    color: #1a1b1f;
    font-weight: 400;
    font-size: 16px;
    padding-top: 80px;

    &-bold {
      color: #191b1e;
      font-size: 54px;
      font-weight: 600;
      letter-spacing: 0.4px;
      line-height: 60px;
      margin: 10px 0;
    }

    &-desc {
      margin: 50px 0 100px;

      &-title {
        font-weight: 500;
        font-size: 18px;
      }
    }
  }

  .text-white-shadow {
    cursor: pointer !important;
    color: #ffffff;
    text-shadow: 1px 1px 1px #000, 0 -1px 1px #000, 1px 1px 1px #000, -1px 0 0 #000, 1px 1px 0 #000, 1px 0 0 #000, 0 -1px 0 #000;

    .typed {
      color: #ffffff !important;
    }
  }

  .text-yellow {
    cursor: pointer !important;
    background-color: #fffaa3;
    color: #191b1e;
    text-shadow: none;
  }

  .text-white-shadow-hover:hover {
    color: #ffffff;
    background-color: transparent;
    text-shadow: 1px 1px 1px #000, 0 -1px 1px #000, 1px 1px 1px #000, -1px 0 0 #000, 1px 1px 0 #000, 1px 0 0 #000, 0 -1px 0 #000;
  }

  .text-blue:hover {
    background-color: #a8ecff;
    color: #191b1e;
    text-shadow: none;
  }

  .text-orange:hover {
    background-color: #ffd297;
    color: #191b1e;
    text-shadow: none;
  }

  .text-green {
    cursor: pointer !important;

    &:hover {
      background-color: #cefe9d;
      color: #191b1e;
      text-shadow: none;

      .typed {
        color: #191b1e !important;
      }
    }
  }
</style>
