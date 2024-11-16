<template>

  <!-- Navigation Bar -->
  <v-app-bar absolute flat :style="{ backgroundColor: 'rgba(250,31,31,0.45)' }">
    <v-spacer></v-spacer>
    <v-btn variant="text" class="text-white" @click="">Home</v-btn>
    <v-btn variant="text" class="text-white" @click="">Impressum</v-btn>
    <v-btn variant="text" class="text-white" @click="">Datenschutz</v-btn>
    <v-spacer></v-spacer>
  </v-app-bar>

  <!-- Text Content -->
  <div class="mx-auto" style="margin-top: 100px; max-width: 1400px">
    <h1 class="heading display-2 text-center font-weight-bold mb-3 text-black text-uppercase">Impressum</h1>
  </div>

  <div class="content">
    <h2 style="padding-left: 20px;">1. Majorettencorps Berlin e. V. • Les Amis - Die Freunde</h2>
    <h3 style="padding-left: 20px;">Postadresse</h3>
    <p style="padding-left: 20px;">
      Falkentaler Steig 36
      D-13467 Berlin, Deutschland
    </p>
    <h3 style="padding-left: 20px;">Telefon</h3>
    <p style="padding-left: 20px;">
      0151 - 41 95 30 66
    </p>
    <h3 style="padding-left: 20px;">E-Mail</h3>
    <p style="padding-left: 20px;">
      <strong>Allgemeine Informationen:</strong><br>
      info@majorettencorps.de<br>
      <strong>Vorstand:</strong><br>
      vorstand@majorettencorps.de
    </p>

    <p class="mt-4" style="padding-left: 20px;">
      <strong>Vertretungsberechtigter Vorstand:</strong><br>
      Nina Eißrich (1. Vorsitzende), Daria Skyschus (2. Vorsitzende), Nicole Schmitz, Jessica Behrend
      <br><br>
      <strong>Registergericht:</strong><br><br>
      Amtsgericht Berlin-Charlottenburg, Registernummer VR 6116Nz
    </p>

    <h3 style="padding-left: 20px;">Haftungshinweis</h3>
    <p style="padding-left: 20px;">Wir übernehmen keine Haftung für die Inhalte externer Links. Für den Inhalt der verlinkten Seiten sind
      ausschließlich deren Betreiber verantwortlich.</p>


  </div>

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
      <v-btn icon="mdi-instagram" href="https://www.instagram.com/1.majorettencorpsberlinlesamis/" class="mx-4"
             variant="text" color="black"></v-btn>
      <v-btn icon="mdi-facebook" href="https://www.tiktok.com/@majorettencorpsberlin?_t=8rRRET4QzUP&_r=1" class="mx-4"
             variant="text" color="black"></v-btn>
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
