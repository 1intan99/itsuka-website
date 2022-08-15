<template>
  <div class="container animate__animated animate__fadeIn">
    <div class="row">
      <div class="col-md-6">
        <div class="about">
          <h1 class="line-after">About Me</h1>
          <h4 class="mt-4">Hey 👋</h4>
          <p>
            My name is Itsuka Kotori, I am a <b>Lightweight </b> and
            <b>Stable </b>. Discord Music Bot For Your Daily Production.
            <u>Discord</u>.
          </p>
          <p>
            I bring you a lot of features to play music from Spotify, Apple
            Music, SoundCloud and more. I can play a recommended music for your
            daily production by running <code>autoplay</code> command.
          </p>
          <h4 class="mt-5">Commands</h4>
          <p>Here is my seperate command that you can use:</p>
          <div class="row animate__animated animate__fadeInUp">
            <div class="col">
              <ul style="list-style-type: circle">
                <li>play</li>
                <li>search</li>
                <li>skip</li>
                <li>stop</li>
                <li>join</li>
                <li>leave</li>
                <li>playlist</li>
                <li>autoplay</li>
                <li>24/7</li>
                <li>bgm</li>
                <li>filter</li>
                <li>loop</li>
                <li>nowplay</li>
                <li>pause</li>
                <li>resume</li>
                <li>queue</li>
                <li>remove</li>
                <li>shuffle</li>
                <li>volume</li>
                <li>lyrics</li>
              </ul>
            </div>
            <div class="col">
              <ul style="list-style-type: circle">
                <li>info</li>
                <li>help</li>
                <li>ping</li>
                <li>invite</li>
              </ul>
            </div>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <img
          src="https://i.imgur.com/UmWcMjO.png"
          alt="Itsuka Wallpaper"
          class="abt-img"
        />
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      startYear: 2021,
      currYear: new Date().getFullYear(),
      stacks: [
        {
          language: "HTML",
          experience: "3+ Years",
          variant: "secondary",
          breif: "lorem...",
        },
        {
          language: "CSS",
          experience: "3+ Years",
          variant: "primary",
          breif: "lorem...",
        },
        {
          language: "Javascript",
          experience: "2+ Years",
          variant: "warning",
          breif: "lorem...",
        },
        {
          language: "VUE.JS",
          experience: "2+ Years",
          variant: "success",
          breif: "lorem...",
        },
        {
          language: "Node.js",
          experience: "2+ Years",
          variant: "dark",
          breif: "lorem...",
        },
      ],
    };
  },
  head: {
    title: "About - Itsuka",
    meta: [
      {
        hid: "description",
        name: "description",
        // currYear - startYear
        content: `A Lightweight and Stable Discord Music Bot For Your Daily Production.`,
      },
    ],
  },
};
</script>
<style scoped>
.container {
  margin-top: 140px;
  text-align: left;
}
.line-after {
  overflow: hidden;
}
.line-after::after {
  content: "";
  display: inline-block;
  height: 0.5em;
  vertical-align: bottom;
  width: 100%;
  margin-right: -100%;
  margin-left: 10px;
  border-top: 2px solid rgb(211, 46, 46);
}
.abt-img {
  width: inherit;
  height: inherit;
  border-radius: 5px;
}
/* .abt-img:hover {
  animation: swing;
  animation-duration: 2s;
} */
</style>
