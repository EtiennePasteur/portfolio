<template>
  <div class="work">
    <div class="work-header background-blue">
      <div class="container d-flex justify-content-center align-items-center">
        <img alt="neo9" class="img-neo9" src="~/assets/img/Neo9.png" />
      </div>
    </div>
    <div class="work-body">
      <div class="container">
        <div class="work-body-title">AprilOn</div>
        <div class="work-body-desc d-flex flex-row justify-content-between">
          <div class="overview d-flex flex-column">
            <div class="overview-title">
              OVERVIEW
            </div>
            <div class="overview-desc">
              <div>Intégrer à une équipe d'une dizaine de développeurs, j'ai participé au développement de l'extranet courtier d'APRIL (AprilOn) ainsi qu'au développement de sa Marketplace multi-marque.</div>
              <div>Du lancement du projet jusqu'à sa mise en production, puis durant sa phase d'exploitation, j'ai eu la chance de passer par toutes les phases de vie du projet.</div>
            </div>
          </div>
          <div class="role d-flex flex-column">
            <div class="role-title">
              MY ROLE
            </div>
            <div class="role-desc"></div>
          </div>
        </div>
      </div>
    </div>
    <div class="spacer"></div>
  </div>
</template>

<style lang="scss">
  .work {
    font-family: 'Avenir Next', sans-serif;

    .background-blue {
      background-color: #99cbfa;

      div {
        padding: 80px 0;

        .img-neo9 {
          width: 560px;
        }
      }
    }

    &-body {
      margin: 60px 0;

      &-title {
        font-weight: 600;
        font-size: 3vw;
        line-height: 3.5vw;
        letter-spacing: 0.4px;
        padding-bottom: 50px;
      }

      &-desc {
        .overview {
          flex: 2;
          margin-right: 30px;

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
          flex: 1;
          margin-left: 30px;

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
