<template>
  <div class="home">
    <v-row justify="space-between" no-gutters>
      <v-col
        cols="12"
        sm="6"
        md="3"
        xs="6"
        v-for="post in recentPost"
        :key="post.id"
      >
        <v-card outlined>
          <v-img
            class="white--text align-end"
            height="200px"
            src="../assets/images/t5.jpg"
          >
            <v-card-title class="head-post-title">{{
              post.title
            }}</v-card-title>
          </v-img>
        </v-card>
      </v-col>
    </v-row>

    <!-- <div class="d-flex justify-space-between">
      
      <v-card max-width="410" outlined>
        <v-img
          class="white--text align-end"
          height="250px"
          src="https://cdn.vuetifyjs.com/images/cards/docks.jpg"
        >
          <v-card-title>Top 10 Australian beaches</v-card-title>
        </v-img>
      </v-card>
      <v-card max-width="410" outlined>
        <v-img
          class="white--text align-end"
          height="250px"
          src="https://cdn.vuetifyjs.com/images/cards/docks.jpg"
        >
          <v-card-title>Top 10 Australian beaches</v-card-title>
        </v-img>
      </v-card>
      <v-card max-width="410" outlined>
        <v-img
          class="white--text align-end"
          height="250px"
          src="https://cdn.vuetifyjs.com/images/cards/docks.jpg"
        >
          <v-card-title>Top 10 Australian beaches</v-card-title>
        </v-img>
      </v-card>
    </div> -->
    <div style="text-align:center;" class="mt-5">
      <img src="../assets/adds.jpg" alt="adds" width="100%" />
    </div>
    <div>
      <v-container>
        <v-row justify="space-between">
          <v-col cols="12" sm="6" md="4" xs="12">
            <v-card outlined>
              <v-img
                src="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg"
                height="200px"
              ></v-img>
              <v-card-text>
                <v-chip class="ma-2" label color="#D1ECF6">News</v-chip>
                <v-chip class="ma-2" label color="#D1ECF6">Read</v-chip>
              </v-card-text>
              <v-card-title>
                Academy Launches New Conversation Series On Race And Gender
                Equity in Filmmaking “Academy Dialogues: It Starts With Us”
              </v-card-title>

              <v-card-subtitle>
                Conversations about race, ethnicity, gender, history,
                opportunity and the art of filmmaking
              </v-card-subtitle>
            </v-card>
          </v-col>
          <v-col cols="12" sm="6" md="4" xs="12">
            <v-card outlined>
              <v-img
                src="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg"
                height="200px"
              ></v-img>
              <v-card-text>
                <v-chip class="ma-2" label color="#D1ECF6">Interviews</v-chip>
                <v-chip class="ma-2" label color="#D1ECF6">News</v-chip>
                <v-chip class="ma-2" label color="#D1ECF6">Read</v-chip>
              </v-card-text>
              <v-card-title>
                Stan Shaw Talks New Horror/Western Film ‘The Pale Door’
              </v-card-title>

              <v-card-subtitle>
                RLJE Films and Shudder will release the horror / Western THE
                PALE DOOR in theaters and On Demand and Digital on August 21,
                2020.
              </v-card-subtitle>
            </v-card>
          </v-col>
          <v-col cols="12" sm="6" md="4" xs="12">
            <img
              src="../assets/filmad.jpg"
              alt="ads"
              height="400px;"
              width="100%"
            />
          </v-col>
        </v-row>
      </v-container>
    </div>

    <!-- Editors Pick -->
    <div>
      <v-container>
        <span class="category_span">
          Editors Picks
        </span>
        <v-row justify="space-between">
          <v-col cols="12" sm="6" md="4" xs="12">
            <v-card outlined>
              <v-img
                src="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg"
                height="200px"
              ></v-img>
              <v-card-text>
                <v-chip class="ma-2" label color="#D1ECF6">News</v-chip>
                <v-chip class="ma-2" label color="#D1ECF6">Read</v-chip>
              </v-card-text>
              <v-card-title>
                Michelle Buteau Lands First Hour-Long Comedy Special on Netflix
              </v-card-title>

              <v-card-subtitle>
                Conversations about race, ethnicity, gender, history,
                opportunity and the art of filmmaking
              </v-card-subtitle>
            </v-card>
          </v-col>
          <v-col cols="12" sm="6" md="4" xs="12">
            <v-card outlined>
              <v-img
                src="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg"
                height="200px"
              ></v-img>
              <v-card-text>
                <v-chip class="ma-2" label color="#D1ECF6">Interviews</v-chip>
                <v-chip class="ma-2" label color="#D1ECF6">News</v-chip>
                <v-chip class="ma-2" label color="#D1ECF6">Read</v-chip>
              </v-card-text>
              <v-card-title>
                Exclusive: Filmmaker Chyna Robinson Talks No Ordinary Love,
                Relationships, and Survival
              </v-card-title>

              <v-card-subtitle>
                RLJE Films and Shudder will release the horror / Western THE
                PALE DOOR in theaters and On Demand and Digital on August 21,
                2020.
              </v-card-subtitle>
            </v-card>
          </v-col>
          <v-col cols="12" sm="6" md="4" xs="12">
            <v-card outlined>
              <v-img
                src="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg"
                height="200px"
              ></v-img>
              <v-card-text>
                <v-chip class="ma-2" label color="#D1ECF6">Interviews</v-chip>
                <v-chip class="ma-2" label color="#D1ECF6">News</v-chip>
                <v-chip class="ma-2" label color="#D1ECF6">Read</v-chip>
              </v-card-text>
              <v-card-title>
                Stan Shaw Talks New Horror/Western Film ‘The Pale Door’
              </v-card-title>

              <v-card-subtitle>
                RLJE Films and Shudder will release the horror / Western THE
                PALE DOOR in theaters and On Demand and Digital on August 21,
                2020.
              </v-card-subtitle>
            </v-card>
          </v-col>
        </v-row>

        <v-row justify="space-between">
          <v-col cols="12" sm="6" md="4" xs="12">
            <v-card outlined>
              <v-img
                src="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg"
                height="200px"
              ></v-img>
              <v-card-text>
                <v-chip class="ma-2" label color="#D1ECF6">News</v-chip>
                <v-chip class="ma-2" label color="#D1ECF6">Read</v-chip>
              </v-card-text>
              <v-card-title>
                Michelle Buteau Lands First Hour-Long Comedy Special on Netflix
              </v-card-title>

              <v-card-subtitle>
                Conversations about race, ethnicity, gender, history,
                opportunity and the art of filmmaking
              </v-card-subtitle>
            </v-card>
          </v-col>
          <v-col cols="12" sm="6" md="4" xs="12">
            <v-card outlined>
              <v-img
                src="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg"
                height="200px"
              ></v-img>
              <v-card-text>
                <v-chip class="ma-2" label color="#D1ECF6">Interviews</v-chip>
                <v-chip class="ma-2" label color="#D1ECF6">News</v-chip>
                <v-chip class="ma-2" label color="#D1ECF6">Read</v-chip>
              </v-card-text>
              <v-card-title>
                Exclusive: Filmmaker Chyna Robinson Talks No Ordinary Love,
                Relationships, and Survival
              </v-card-title>

              <v-card-subtitle>
                RLJE Films and Shudder will release the horror / Western THE
                PALE DOOR in theaters and On Demand and Digital on August 21,
                2020.
              </v-card-subtitle>
            </v-card>
          </v-col>
          <v-col cols="12" sm="6" md="4" xs="12">
            <v-card outlined>
              <v-img
                src="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg"
                height="200px"
              ></v-img>
              <v-card-text>
                <v-chip class="ma-2" label color="#D1ECF6">Interviews</v-chip>
                <v-chip class="ma-2" label color="#D1ECF6">News</v-chip>
                <v-chip class="ma-2" label color="#D1ECF6">Read</v-chip>
              </v-card-text>
              <v-card-title>
                Stan Shaw Talks New Horror/Western Film ‘The Pale Door’
              </v-card-title>

              <v-card-subtitle>
                RLJE Films and Shudder will release the horror / Western THE
                PALE DOOR in theaters and On Demand and Digital on August 21,
                2020.
              </v-card-subtitle>
            </v-card>
          </v-col>
        </v-row>
      </v-container>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Home',
  data() {
    return {
      recentPost: [
        {
          id: 1,
          image:
            'https://www.blackfilm.com/read/2020/09/netflix-now-streaming-all-8-seasons-of-girlfriends/',
          title: 'Netflix Now Streaming All 8 Seasons of Girlfriends',
        },
        {
          id: 2,
          image:
            'https://www.blackfilm.com/read/2020/09/nickelodeon-pulls-their-newest-nick-jr-show-made-by-maddie-amid-hair-love-controversy/',
          title: 'Ghana must go storms Accra Siver Bird Cinemas',
        },
        {
          id: 3,
          image:
            'https://www.blackfilm.com/read/2020/09/nickelodeon-pulls-their-newest-nick-jr-show-made-by-maddie-amid-hair-love-controversy/',
          title: 'Majid Michel inspires in new movie Comic City',
        },
        {
          id: 4,
          image:
            'https://www.blackfilm.com/read/2020/09/nickelodeon-pulls-their-newest-nick-jr-show-made-by-maddie-amid-hair-love-controversy/',
          title: 'Meet the new MTN abassador in kumahood',
        },
      ],
    };
  },
};
</script>
