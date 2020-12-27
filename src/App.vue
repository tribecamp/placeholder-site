<template>
  <div id="app">
    <navbar-container />
    <div class="container">
      <img
        class="illustration"
        src="~@/assets/illustration.svg"
        alt="Illustration"
      >
      <h1 class="header">
        Binnenkort beschikbaar
      </h1>
      <p class="desc">
        Ontdek een moderne online schoolomgeving met een oog voor privacy,
        transparantie en gebruiksvriendelijkheid.
      </p>
      <a class="btnJoinDiscord" href="https://discord.gg/k8cfqZkhqZ">
        <i class="fab fa-discord" />
        <span>Join onze Discord-server</span>
      </a>
      <social-container class="socialContainer" />
    </div>
  </div>
</template>

<script>
import NavbarContainer from './components/NavbarContainer.vue';
import SocialContainer from './components/SocialContainer.vue';

export default {
  components: {
    SocialContainer,
    NavbarContainer
  }
};
</script>

<style lang="scss">
#app {
  font-family: Nunito, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
html,
body {
  margin: 0;
  padding: 0;

  @media (prefers-color-scheme: dark) {
    background-color: #1d1d1d;
  }
}
</style>

<style lang="scss" scoped>
.socialContainer {
  margin-top: 10px;
}

html {
  font-family: Nunito;
}

a {
  color: #00bfff;
  margin-bottom: 5px;
}

.container {
  text-align: center;
  padding: 120px 20px;

  @media (prefers-color-scheme: dark) {
    color: #dfdfdf;
  }

  @media (max-width: 768px) {
    padding-top: 40px;
  }

  .illustration {
    width: 350px;
  }

  .header {
    margin: 15px 0;
    font-size: 52px;
    font-family: Poppins;
  }

  .desc {
    margin: 0 auto;
    padding: 0 15px;
    font-size: 18px;
    max-width: 600px;
  }

  .btnJoinDiscord {
    display: inline-block;
    margin: 20px 0;
    padding: 10px 15px;
    border-radius: 5px;
    background: #7289da;
    color: white;
    text-decoration: none;
    font-weight: bolder;

    i,
    span {
      vertical-align: middle;
    }

    i {
      margin-right: 5px;
    }
  }
}
</style>
