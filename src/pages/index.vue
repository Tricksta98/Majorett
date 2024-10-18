<template>
  <v-parallax :src="getImageUrl('header2.jpg')" height="100vh">
    <!-- Navigation Bar -->
    <v-app-bar absolute flat :style="{ backgroundColor: 'rgba(255, 255, 255, 0.1)' }">
      <v-spacer></v-spacer>
      <v-btn variant="text" class="text-white" @click="">Home</v-btn>
      <v-btn variant="text" class="text-white" @click="">Impressum</v-btn>
      <v-btn variant="text" class="text-white" @click="">Datenschutz</v-btn>
      <v-spacer></v-spacer>
    </v-app-bar>

    <!-- Text Content -->
    <v-row class="header-container" align="center" justify="center">
      <v-col cols="12">
        <div class="mx-auto" style="max-width: 1400px">
          <h1 class="heading display-2 font-weight-bold mb-3 text-white text-uppercase">1. Majorettencorps Berlin
            e.V.</h1>

          <p class="subheading font-weight-regular text-white pl-4">Les Amis - Die Freunde</p>

          <v-btn variant="outlined" class="text-white mt-10 ml-4" size="large"
                 :style="{ backgroundColor: 'transparent', borderColor: 'white' }" @click="scrollDown">
            Mehr Erfahren
          </v-btn>
        </div>
      </v-col>
    </v-row>


  </v-parallax>

  <v-row class="bgc" style="padding-top: 80px; padding-bottom:80px;">
    <v-col cols="4">
      <v-card elevation="5" class="mx-auto bg-white" max-width="350">
        <v-img
            color="surface-variant"
            height="200"
            :src="getImageUrl('gallery1.jpg')"
            cover
        >
        </v-img>

        <v-card-text>
          <h2 class="">Willkommen beim 1. Majorettencorps Berlin e.V.
            Les Amis - Die Freunde</h2>
          <p class="mt-4">Suchen Sie für Ihre Veranstaltung ein High-Light?
            Dann sind unsere Majoretten bestimmt das richtige für Sie!
            Durch unsere Auftritte finanzieren wir Ausrüstung,
            Kostüme und die Fahrten zu Turnieren und Meisterschaften. </p>
        </v-card-text>
      </v-card>
    </v-col>
    <v-col cols="4">
      <v-card elevation="5" class="mx-auto bg-white" max-width="350">
        <v-img
            color="surface-variant"
            height="200"
            :src="getImageUrl('header.jpg')"
            cover
        >
        </v-img>

        <v-card-text>
          <h2 class="">Willkommen beim 1. Majorettencorps Berlin e.V.
            Les Amis - Die Freunde</h2>
          <p class="mt-4">Suchen Sie für Ihre Veranstaltung ein High-Light?
            Dann sind unsere Majoretten bestimmt das richtige für Sie!
            Durch unsere Auftritte finanzieren wir Ausrüstung,
            Kostüme und die Fahrten zu Turnieren und Meisterschaften. </p>
        </v-card-text>
      </v-card>
    </v-col>
    <v-col cols="4">
      <v-card elevation="5" class="mx-auto bg-white" max-width="350">
        <v-img
            color="surface-variant"
            height="200"
            :src="getImageUrl('gallery2.jpg')"
            cover
        >
        </v-img>

        <v-card-text>
          <h2 class="">Willkommen beim 1. Majorettencorps Berlin e.V.
            Les Amis - Die Freunde</h2>
          <p class="mt-4">Suchen Sie für Ihre Veranstaltung ein High-Light?
            Dann sind unsere Majoretten bestimmt das richtige für Sie!
            Durch unsere Auftritte finanzieren wir Ausrüstung,
            Kostüme und die Fahrten zu Turnieren und Meisterschaften. </p>
        </v-card-text>
      </v-card>
    </v-col>
  </v-row>

  <v-row class="mt-12 mb-6">
    <v-col>
      <h2 style="font-size: 40px;" class="text-center">Wir sind Deutscher Meister 2016 in 5 Kategorien!</h2>
      <p class="mt-4 text-center">Unsere Erfolge bei der Deutschen Meisterschaft für Majoretten vom 1. und 2. Oktober 2016 in Berlin</p>
    </v-col>
  </v-row>

  <v-row class="pb-12" align="center" justify="center">
    <v-col cols="12" style="max-width: 800px;">
      <div class="text-center" style="max-width: 800px;">
        <video width="100%" autoplay muted loop>
          <source :src="getVideoUrl('galleryvid1.mp4')" type="video/mp4">
          Your browser does not support the video tag.
        </video>
      </div>
    </v-col>
  </v-row>

  <v-row class="bgc" justify="center" align="center">
    <v-col class="py-12 pr-6 pl-6 text-center" cols="6">
      <h2 class="text-center text-black">Wir sind sicher, daß wir durch
        unseren Auftritt Ihr Fest bereichern
        und Ihre Gäste begeistern werden !!</h2>
      <p class="text-center text-black mt-4">Wir tanzen und marschieren in unserer rot-weißen Gardeuniform, für unsere
        Showtänze haben wir schicke Tanzkostüme in unserem Fundus.
        Überzeugen Sie sich selbst von unserem Können.
        Auf dieser Internetseite finden Sie viele Informationen und Bilder von und über
        uns, oder treffen Sie uns bei einem unserer Auftritte, wie z. B. bei Straßenfesten.
        Wir sind sicher, daß wir durch </p>
    </v-col>
    <v-col class="py-12 text-center" cols="6">
      <v-img :src="getImageUrl('gallery1.jpg')" width="100%" height="400px"></v-img>
    </v-col>
  </v-row>

  <v-row class="py-12" align="center" justify="center">
    <v-col cols="12" style="max-width: 800px;">
      <div class="text-center" style="max-width: 800px;">
        <h2>Kontaktiere uns jetzt!</h2>
        <v-btn color="red" class="text-white mt-4" href="mailto:info@majorettencorps.de">Kontaktieren</v-btn>
      </div>
    </v-col>
  </v-row>

  <v-footer
      class="bgc text-center d-flex flex-column"
  >
    <div>
      <v-btn icon="mdi-instagram" class="mx-4" variant="text" color="black"></v-btn>
      <v-btn icon="mdi-twitter" class="mx-4" variant="text" color="black"></v-btn>
      <v-btn icon="mdi-facebook" class="mx-4" variant="text" color="black"></v-btn>
    </div>

    <div class="pt-0 text-black">
      Les Amis - Die Freunde
    </div>

    <v-divider></v-divider>

    <div class="text-black">
      {{ new Date().getFullYear() }} — <strong>1. Majorettencorps Berlin e.V.</strong>
    </div>
  </v-footer>

</template>

<script>
export default {
  name: "HeadSection",
  methods: {
    getImageUrl(name) {
      return `${import.meta.env.BASE_URL}img/${name}`;
    },
    getVideoUrl(name) {
      return `${import.meta.env.BASE_URL}video/${name}`;
    },
    scrollDown() {
      window.scrollTo({
        top: window.innerHeight,
        behavior: 'smooth'
      });
    },
  }
}
</script>

<style scoped>
.parallax__content {
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
}

/* Make sure your text stands out over the parallax image */
.display-2 {
  color: #fff;
  text-shadow: 0 0 10px rgba(0, 0, 0, 0.7);
  font-size: 82px;
}

.subheading {
  color: #fff;
  text-shadow: 0 0 5px rgba(0, 0, 0, 0.7);
  font-size: 32px;
}

.header-container {
  height: 100%;
}

.default-red {
  color: #d30303;
}

.bgc {
  background-color: #d2d0dd;
}
</style>
