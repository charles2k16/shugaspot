<template>
  <v-app>
    <v-app-bar app dark color="#01101A">
      <div class="d-flex align-center">
        <v-btn text x-large>
          SHUGASPOT.COM
        </v-btn>
      </div>

      <v-spacer></v-spacer>

      <v-btn text>
        News
      </v-btn>
      <v-btn text>
        Reveiews
      </v-btn>
      <v-btn text>
        Interviews
      </v-btn>
      <v-btn text>
        Celebspot
      </v-btn>
      <v-btn text>
        TVS
      </v-btn>
      <v-btn text>
        Gallery/photos
      </v-btn>
      <v-btn icon>
        <v-icon>mdi-magnify</v-icon>
      </v-btn>
      <v-spacer></v-spacer>
      <v-btn icon>
        <v-icon>mdi-facebook</v-icon>
      </v-btn>
      <v-btn icon>
        <v-icon>mdi-twitter</v-icon>
      </v-btn>
      <v-btn icon>
        <v-icon>mdi-instagram</v-icon>
      </v-btn>
    </v-app-bar>

    <v-main>
      <v-alert color="#1F84AB" dark dense>
        <div class="d-flex justify-space-between">
          <v-btn text>GET ALL YOUR MOVIE UPDATES & MORE!</v-btn>
          <v-btn class="black--text" color="white">
            <v-icon left dark>mdi-youtube-subscription</v-icon>
            SUBSCRIBE TO OUR YOUTUBE
          </v-btn>
          <v-btn text>
            <v-icon left dark>mdi-trophy-award</v-icon>
            TELLY SHOW AWARDS
          </v-btn>
        </div>
      </v-alert>
      <router-view />
    </v-main>
  </v-app>
</template>

<script>
export default {
  name: 'App',
  data: () => ({
    //
  }),
};
</script>
