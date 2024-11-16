<template>
  <v-parallax :src="getImageUrl('header1.jpg')" height="100vh">
    <!-- Navigation Bar -->
    <v-app-bar absolute flat :style="{ backgroundColor: 'rgba(250,31,31,0.45)' }">
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
      <v-card elevation="5" class="mx-auto bg-white float-right" max-width="350" min-height="550">
        <v-img
            color="surface-variant"
            height="260"
            :src="getImageUrl('gallery1.jpg')"
            cover
        >
        </v-img>

        <v-card-text>
          <h2 class="">Willkommen beim 1. Majorettencorps Berlin e.V.
            Les Amis - Die Freunde</h2>
          <p class="mt-4">Wir starten wieder in eine neue Saison.
            Majoretten oder auch Baton Twirling genannt, kann man mit Gardetanz vergleichen und dabei dreht und wirft
            man die Twirlingstäbe. Der Stab ist ein ca 50cm langer Metallstab. Es wird nach klassischen Märschen
            getanzt, aber auch zu moderner, aktueller Musik. </p>
        </v-card-text>
      </v-card>
    </v-col>
    <v-col cols="4">
      <v-card elevation="5" class="mx-auto bg-white" max-width="350" min-height="550">
        <v-img
            color="surface-variant"
            height="260"
            :src="getImageUrl('minis1.jpg')"
            cover
        >
        </v-img>

        <v-card-text>
          <h2 class="">Haben wir dein Interesse geweckt?</h2>
          <p class="mt-4">Wir bieten Kinder ab 6 Jahren ein 4 wöchiges, kostenloses Probetraining an.
            Wir trainieren in der großen Turnhalle der Grundschule am Tegelschen Ort, Gerlindeweg 11-23, 13505 Berlin
            Tegelort. Mittwochs von 17-18:30 Uhr.
            Einfach Sportsachen mitbringen und Mittwoch starten.<br> ( In den Ferien findet kein Training statt ).
            <br>Bei Fragen gerne per Mail oder dann vor Ort. Mail: <a href="mailto:info@majorettencorps.de">info@majorettencorps.de</a>
          </p>
        </v-card-text>
      </v-card>
    </v-col>
    <v-col cols="4">
      <v-card elevation="5" class="mx-auto bg-white float-left" max-width="350" min-height="550">
        <v-img
            color="surface-variant"
            height="260"
            :src="getImageUrl('frontal1.jpg')"
            cover
        >
        </v-img>

        <v-card-text>
          <h2 class="">Wir tanzen für Ihr Event</h2>
          <p class="mt-4">Suchen Sie für Ihre Veranstaltung ein High-Light?
            Dann sind unsere Majoretten bestimmt das Richtige für Sie!
            Durch unsere Auftritte finanzieren wir Ausrüstung,
            Kostüme und die Fahrten zu Turnieren und Meisterschaften.
            <br>
            Bei dem Schollenumzug, der jährlich Anfang September in der Freien Scholle stattfindet sind wir seit
            Jahrzehnten auch dabei und tanzen erfolgreich auf Turnieren mit.
            <br>
            Einfach Kontakt per Mail aufnehmen.
          </p>
        </v-card-text>
      </v-card>
    </v-col>
  </v-row>

  <v-row class="mt-12 mb-6">
    <v-col>
      <h2 style="font-size: 40px;" class="text-center default-red">Hier ein paar Einblicke unserer Les Amis Familie</h2>
      <p class="mt-4 text-center default-red">Viel Liebe und viele Emotionen sind immer dabei</p>
    </v-col>
  </v-row>

  <v-row class="pb-12" align="center" justify="center">
    <v-col cols="12" style="max-width: 800px;">
      <div class="text-center" style="max-width: 800px;">
        <video width="400px" controls loop>
          <source :src="getVideoUrl('majorett.mp4')" type="video/mp4">
          Your browser does not support the video tag.
        </video>
      </div>
    </v-col>
  </v-row>

  <v-row class="bgc" justify="center" align="center">
    <v-col class="py-12 pr-6 text-center" style="padding-left: 120px; max-width: 800px; float: right;" cols="6">
      <h2 class="text-left text-black">Willst du wissen wie wir entstanden sind?</h2>
      <p class="text-left text-black mt-4">Das 1. Majorettencorps Berlin, gegründet am 28. Dezember 1978, war einer
        der ersten Vereine seiner Art in Deutschland. Der aus Amerika über Frankreich kommende Sport fand zunächst im
        Rheinland Anschluss an Karnevalsvereine. Nach langem Einsatz gelang es dem Berliner Verein, sich dem Deutschen
        Tanzsportverband und dem Landessportbund anzuschließen sowie als gemeinnützig anerkannt zu werden.
        <br><br>
        Die Mädels unseres Vereins sind erfolgreich im Wettkampfsport und errangen bei der Europameisterschaft 1995 in Viersen fünf Titel
        gegen starke Konkurrenz. Diese Erfolge werden bis heute auf nationalen Meisterschaften
        verteidigt. </p>
    </v-col>
    <v-col class="py-12 text-center" cols="6">
      <v-img :src="getImageUrl('klenen2.jpg')" height="350px"></v-img>
    </v-col>
  </v-row>

  <v-row class="py-12" align="center" justify="center">
    <v-col cols="12" style="max-width: 800px;">
      <div class="text-center" style="max-width: 800px;">
        <h2 class="default-red">Kontaktiere uns jetzt!</h2>
        <v-btn color="red" class="text-white mt-4" href="mailto:info@majorettencorps.de">Kontaktieren</v-btn>
      </div>
    </v-col>
  </v-row>

  <v-footer
      class="bgc text-center d-flex flex-column"
  >
    <div>
      <v-btn icon="mdi-instagram" href="https://www.instagram.com/1.majorettencorpsberlinlesamis/" class="mx-4" variant="text" color="black"></v-btn>
      <v-btn icon="mdi-facebook" href="https://www.tiktok.com/@majorettencorpsberlin?_t=8rRRET4QzUP&_r=1" class="mx-4" variant="text" color="black"></v-btn>
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
  background-color: rgba(255, 179, 179, 0.35);
}
</style>
