<template>
  <div class="under-construction">
    <div class="background-image"></div>
    <div class="content">
      <h1 class="headline">bleibholz</h1>
      <h2 class="subheadline">
        Unsere Seite befindet sich im Aufbau. Komm bald wieder!
      </h2>
    </div>
    <NuxtLink class="impressum_link" to="/impressum"
      >Impressum</NuxtLink
    >
  </div>
</template>

<script>
export default {
  name: 'UnderConstruction',
};
</script>

<style scoped>
/* Style the container */
.under-construction {
  position: relative;
  height: 100vh;
  overflow: hidden;
}

.background-image {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-image: url('/img_1.jpg');
  /* Replace with your image URL */
  background-size: cover;
  background-position: center;
  filter: brightness(40%);
  /* Adjust the brightness as needed */
}

/* Style the content */
.content {
  position: absolute;
  top: 30%;
  left: 50%;
  transform: translate(-50%, -50%);
  text-align: center;
  color: white;
}

.headline {
  font-size: 6em;
  margin-bottom: 10px;
  font-family: 'Smooch', cursive;
}

/* Media query for screens 600px and smaller */
@media only screen and (min-width: 600px) {
  .headline {
    font-size: 4em;
  }
}

/* Media query for screens 768px and smaller */
@media only screen and (min-width: 768px) {
  .headline {
    font-size: 5em;
  }
}

/* Media query for screens 1024px and smaller */
@media only screen and (min-width: 1024px) {
  .headline {
    font-size: 8em;
  }
}

.subheadline {
  font-size: 1.5em;
  font-weight: normal;
}

.impressum_link {
  position: absolute;
  bottom: 30px;
  right: 20px;
  color: #ffffff;
  text-decoration: none;
  font-size: 1em;
}
</style>
