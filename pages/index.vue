<template>
  <b-row style="margin-left: 0; margin-right: 0">
    <b-col md="4">
      <b-img
        src="https://images-ext-1.discordapp.net/external/LO-k41aNh_y2TB5K3a4Vh0g6QEE3GEB5TJb-1yXDVRM/%3Fsize%3D4096/https/cdn.discordapp.com/avatars/477762276389027840/f1a56f884fe1edc46ae81d8711b33b57.png?width=636&height=636"
        id="avatar-img"
        alt="Itsuka"
      />
    </b-col>

    <b-col md="8">
      <h2 class="intro animate__animated animate__fadeInUp animate__fast">
        Hi!,
        <br />I<span>'m Itsuka</span>.
      </h2>

      <div class="col-md-10 info">
        A <b>Lightweigh</b> and <b>Stable</b> Discord Music Bot For Your Daily
        Production.
        <br />
        <b-button
          class="action-btn animate__animated animate__wobble animate__delay-4s animate__fast"
          to="/about"
        >
          Explore >
        </b-button>

        <b-button
          class="action-btn"
          href="https://discord.gg/h67nbaqdVm"
          variant="primary"
          target="_blank"
        >
          Get In Touch
        </b-button>

        <!-- .SOCIAL LINKS SECTION -->
        <div
          class="social-icons animate__animated animate__fadeInUp animate__delay-1s"
        >
          <social-link :to="socialLinks.github">
            <GithubIcon />
          </social-link>

          <social-link :to="socialLinks.youtube">
            <YoutubeIcon />
          </social-link>
        </div>
      </div>
    </b-col>
  </b-row>
</template>

<script>
import GithubIcon from "vue-ionicons/dist/logo-github.vue";
import LinkedinIcon from "vue-ionicons/dist/logo-linkedin.vue";
import TwitterIcon from "vue-ionicons/dist/logo-twitter.vue";
import FacebookIcon from "vue-ionicons/dist/logo-facebook.vue";
import YoutubeIcon from "vue-ionicons/dist/logo-youtube.vue";
import MailIcon from "vue-ionicons/dist/md-mail.vue";

export default {
  components: {
    GithubIcon,
    LinkedinIcon,
    TwitterIcon,
    FacebookIcon,
    YoutubeIcon,
    MailIcon,
  },

  data() {
    return {
      avatar: require("@/assets/avatar-1.webp"),
      // ADD YOUR SOCIAL LINKS HERE 👇
      socialLinks: {
        github: "https://github.com/Yukkuri-Studio/yukkuri-lava",
        youtube: "https://1intan99.my.id/youtube",
      },
    };
  },

  head: {
    title: "Itsuka Dashbord",
    meta: [
      {
        hid: "description",
        name: "description",
        content:
          "A Lightweight and Stable Discord Music Bot For Your Daily Production.",
      },
      {
        hid: "og:title",
        name: "og:title",
        content: "Itsuka Dashbord",
      },
      {
        property: "og:description",
        content:
          "A Lightweight and Stable Discord Music Bot For Your Daily Production.",
      },
      {
        hid: "og:image",
        name: "og:image",
        content: "https://i.imgur.com/UmWcMjO.png",
      },
    ],
  },
  mounted() {
    this.$nextTick(() => {
      this.$nuxt.$loading.start();

      setTimeout(() => this.$nuxt.$loading.finish(), 500);
    });
  },
};
</script>
