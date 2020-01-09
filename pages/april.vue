<template>
  <div class="work">
    <div class="work-header background-blue">
      <div class="aspect-ratio">
        <div class="work-container d-flex justify-content-center align-items-center">
          <img alt="neo9" class="img-neo9" src="~/assets/img/Neo9.png" />
        </div>
      </div>
    </div>
    <div class="work-body">
      <div class="container">
        <div class="work-body-title">AprilOn</div>
        <div class="work-body-desc row m-0">
          <div class="overview d-flex flex-column col-md-8">
            <div class="overview-title">OVERVIEW</div>
            <div class="overview-desc">
              <div>Intégrer à une équipe d'une dizaine de développeurs, j'ai participé au développement de l'extranet courtier d'APRIL (AprilOn) ainsi qu'au développement de sa Marketplace multi-marque.</div>
              <div>Du lancement du projet jusqu'à sa mise en production, puis durant sa phase d'exploitation, j'ai eu la chance de passer par toutes les phases de vie du projet.</div>
            </div>
          </div>
          <div class="role d-flex flex-column col-md-4 mt-5 mt-md-0">
            <div class="role-title">MY ROLE</div>
            <div class="role-desc d-flex flex-column">
              <div class="role-desc-position">Fullstack developer</div>
              <div class="role-desc-desc pt-2">Front-end development using Angular 7, Back-end development with Java Spring Boot</div>
              <div class="role-desc-time pt-4">March 2019 - January 2020</div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="spacer"></div>
  </div>
</template>

<style lang="scss" scoped>
  .work {
    font-family: 'Avenir Next', sans-serif;

    .aspect-ratio {
      padding-bottom: 45%;

      @media (min-width: 992px) {
        padding-bottom: 25%;
      }
    }

    &-header {
      position: relative;
    }

    &-container {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
    }

    .background-blue {
      background-color: #99cbfa;

      div {
        .img-neo9 {
          height: 65%;
        }
      }
    }

    &-body {
      margin: 60px 0;

      &-title {
        font-weight: 600;
        letter-spacing: 0.4px;
        font-size: 22px;
        padding-bottom: 50px;

        @media (min-width: 576px) {
          font-size: 30px;
        }

        @media (min-width: 768px) {
          font-size: 36px;
        }

        @media (min-width: 992px) {
          font-size: 42px;
        }

        @media (min-width: 1200px) {
          font-size: 50px;
        }
      }

      &-desc {
        .overview {
          padding: 0;

          @media (min-width: 768px) {
            padding-right: 30px;
          }

          &-title {
            color: #757678;
            font-size: 14px;
            line-height: 24px;
            font-weight: 400;
            letter-spacing: 1px;
            text-transform: uppercase;
            margin-bottom: 20px;
          }
        }

        .role {
          padding: 0;

          @media (min-width: 768px) {
            padding-left: 30px;
          }

          &-title {
            color: #757678;
            font-size: 14px;
            line-height: 24px;
            font-weight: 400;
            letter-spacing: 1px;
            text-transform: uppercase;
            margin-bottom: 20px;
          }

          &-desc {
            &-position {
              font-weight: bold;
            }
          }
        }
      }
    }

    .spacer {
      margin-right: 100px;
      margin-left: 100px;
      border-style: solid;
      border-width: 0.5px;
      border-color: #ccc;
    }
  }
</style>
