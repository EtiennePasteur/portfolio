<template>
  <div class="footer">
    <div class="container d-flex justify-content-center align-items-center flex-column">
      <div class="footer-title">Let's connect</div>
      <div class="footer-desc text-center">Get in touch for opportunities or just to say hi! 👋</div>
      <div class="social d-flex flex-row justify-content-between align-items-center">
        <a href="https://github.com/EtiennePasteur" target="_blank">
          <fa :icon="['fab', 'github-square']" />
        </a>
        <a href="mailto:me@etiennepasteur.com" target="_blank">
          <fa :icon="['fas', 'at']" />
        </a>
        <a href="https://linkedin.com/in/etiennepasteur" target="_blank">
          <fa :icon="['fab', 'linkedin']" />
        </a>
      </div>
    </div>
  </div>
</template>
<style scoped lang="scss">
  .footer {
    font-family: 'Avenir Next', sans-serif;
    margin: 100px 0;

    &-title {
      font-weight: 600;
      font-size: 26px;
    }

    .social {
      font-size: 42px;
      width: 220px;
      margin-top: 30px;

      a {
        color: #191b1e;
        text-decoration: none;

        &:hover {
          opacity: 0.5;
          transform: scale(1.05);
        }
      }
    }
  }
</style>
