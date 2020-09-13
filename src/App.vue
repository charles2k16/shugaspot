<template>
  <v-app>
    <v-row no-gutters style="background-color: #00182A;">
      <v-col cols="12" sm="12" md="12" xs="12">
        <div class="d-flex-justify-between">
          <span>
            <v-btn text x-large class="d-none d-md-flex" dark>
              SHUGASPOT.COM
            </v-btn>
            <v-app-bar-nav-icon
              @click.stop="drawer = !drawer"
              style="color:white;"
              class="d-flex d-sm-none"
            ></v-app-bar-nav-icon>
          </span>

          <span class="d-flex d-sm-none">
            <v-btn text x-large dark>
              SHUGASPOT.COM
            </v-btn>
          </span>

          <span class="d-flex d-sm-none">
            <v-btn icon dark>
              <v-icon>mdi-magnify</v-icon>
            </v-btn>
          </span>

          <span class="d-none d-md-flex">
            <v-btn text dark v-for="item in menuItems" :key="item.title">
              {{ item.title }}
            </v-btn>
          </span>

          <span class="d-none d-md-flex">
            <v-btn icon dark>
              <v-icon>mdi-facebook</v-icon>
            </v-btn>
            <v-btn icon dark>
              <v-icon>mdi-twitter</v-icon>
            </v-btn>
            <v-btn icon dark>
              <v-icon>mdi-instagram</v-icon>
            </v-btn>
          </span>
        </div>
      </v-col>
    </v-row>
    <!-- <v-app-bar app dark color="#01101A" style="width: 100%"> </v-app-bar> -->

    <v-navigation-drawer
      color="#00182A"
      height="100%"
      class="d-flex d-sm-none"
      dark
      absolute
      v-model="drawer"
    >
      <div style="text-align: center;" class="mt-5">
        <v-btn icon>
          <v-icon left dark>mdi-close</v-icon>
        </v-btn>
      </div>
      <v-list>
        <v-list-item v-for="item in menuItems" :key="item.title" link>
          <v-list-item-icon>
            <v-icon small>{{ item.icon }}</v-icon>
          </v-list-item-icon>

          <v-list-item-content>
            <v-list-item-title class="subtitle-2">{{
              item.title
            }}</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
      <hr />
      <div class="mt-5">
        <v-btn icon dark class="mr-3">
          <v-icon>mdi-facebook</v-icon>
        </v-btn>
        <v-btn icon dark class="mr-3">
          <v-icon>mdi-twitter</v-icon>
        </v-btn>
        <v-btn icon dark>
          <v-icon>mdi-instagram</v-icon>
        </v-btn>
      </div>
      <div class="mt-4">
        <v-btn class="white--text" color="red" x-small>
          <v-icon left dark>mdi-youtube-subscription</v-icon>
          SUBSCRIBE TO OUR YOUTUBE
        </v-btn>
      </div>
    </v-navigation-drawer>

    <v-main>
      <v-alert color="#1F84AB" dark dense class="d-none d-md-flex">
        <div class="d-flex-justify-between">
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
    drawer: false,
    menuItems: [
      { title: 'NEWS', icon: 'mdi-newspaper', route: '/news' },
      { title: 'REVIEWS', icon: 'mdi-printer-eye', route: '/reviews' },
      {
        title: 'INTERVIEWS',
        icon: 'mdi-camera-wireless-outline',
        route: '/interviews',
      },
      { title: 'CELEBSPOT', icon: 'mdi-spotlight', route: '/interviews' },
      { title: 'TVS', icon: 'mdi-gavel', route: '/interviews' },
      {
        title: 'GALLERY/PHOTOS',
        icon: 'mdi-image-multiple',
        route: '/interviews',
      },
    ],
  }),
};
</script>
