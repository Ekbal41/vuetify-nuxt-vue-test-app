<script lang="ts" setup></script>

<template>
  <v-container style="max-width: 1500px">
    <v-card class="d-flex mt-16 pa-4 align-center justify-center" variant="tonal">
      <v-flex>
        <div class="ml-4">
          <v-avatar size="150">
            <img src="https://cdn.vuetifyjs.com/images/john.jpg" alt="Vuetify Logo">
          </v-avatar>
        </div>
        <div class="d-flex flex-column align-center justify-center mt-5">
          <v-card-title class="text-h5">Asif Ekbal</v-card-title>
          <v-card-subtitle class="text-h6">No name person</v-card-subtitle>
        </div>
      </v-flex>
    </v-card>

    <v-layout class=" mt-16">

      <v-row>
        <v-col cols="12" md="6">

          <v-list>
            <v-list-item class="mt-5">
              <v-list-item-icon>
                <v-icon>mdi-map-marker</v-icon>
              </v-list-item-icon>
              <v-list-item-content>
                <v-list-item-title>Location</v-list-item-title>
                <v-list-item-subtitle>San Francisco, CA</v-list-item-subtitle>
              </v-list-item-content>
            </v-list-item>
            <v-list-item class="mt-5">
              <v-list-item-icon>
                <v-icon>mdi-calendar</v-icon>
              </v-list-item-icon>
              <v-list-item-content>
                <v-list-item-title>Joined</v-list-item-title>
                <v-list-item-subtitle>June 2018</v-list-item-subtitle>
              </v-list-item-content>
            </v-list-item>
            <v-list-item class="mt-5">
              <v-list-item-icon>
                <v-icon>mdi-email</v-icon>
              </v-list-item-icon>
              <v-list-item-content>
                <v-list-item-title>Email</v-list-item-title>
                <v-list-item-subtitle>
                  mageina@gmail.com
                </v-list-item-subtitle>
              </v-list-item-content>
            </v-list-item>
            <v-list-item class="mt-5">
              <v-list-item-icon>
                <v-icon>mdi-phone</v-icon>
              </v-list-item-icon>
              <v-list-item-content>
                <v-list-item-title>Phone</v-list-item-title>
                <v-list-item-subtitle>
                  +1 (555) 123-4567
                </v-list-item-subtitle>
              </v-list-item-content>
            </v-list-item>
          </v-list>
        </v-col>
        <v-divider vertical></v-divider>
        <v-col cols="12" md="6">
          <!-- educational information -->
          <v-list>
            <v-list-item class="mt-5">
              <v-list-item-icon>
                <v-icon>mdi-school</v-icon>
              </v-list-item-icon>
              <v-list-item-content>
                <v-list-item-title>Education</v-list-item-title>
                <v-list-item-subtitle>
                  <v-list-item>
                    <v-list-item-content>
                      <v-list-item-title>University of California, Berkeley</v-list-item-title>
                      <v-list-item-subtitle>B.A. in English</v-list-item-subtitle>
                    </v-list-item-content>
                  </v-list-item>
                  <v-list-item>
                    <v-list-item-content>
                      <v-list-item-title>Harvard University</v-list-item-title>
                      <v-list-item-subtitle>M.A. in Education</v-list-item-subtitle>
                    </v-list-item-content>
                  </v-list-item>
                </v-list-item-subtitle>
              </v-list-item-content>
            </v-list-item>
            <!-- work experience -->
            <v-list-item class="mt-5">
              <v-list-item-icon>
                <v-icon>mdi-briefcase</v-icon>
              </v-list-item-icon>
              <v-list-item-content>
                <v-list-item-title>Work Experience</v-list-item-title>
                <v-list-item-subtitle>
                  <v-list-item>
                    <v-list-item-content>
                      <v-list-item-title>Teacher</v-list-item-title>
                      <v-list-item-subtitle>San Francisco, CA</v-list-item-subtitle>
                    </v-list-item-content>
                  </v-list-item>
                  <v-list-item>
                    <v-list-item-content>
                      <v-list-item-title>Teacher</v-list-item-title>
                      <v-list-item-subtitle>San Francisco, CA</v-list-item-subtitle>
                    </v-list-item-content>
                  </v-list-item>
                </v-list-item-subtitle>
              </v-list-item-content>
            </v-list-item>
          </v-list>

        </v-col>
      </v-row>


    </v-layout>
  </v-container>
</template>

<style scoped></style>
