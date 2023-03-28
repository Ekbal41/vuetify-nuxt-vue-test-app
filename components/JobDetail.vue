<script lang="ts" setup></script>

<template>
  <div>
    <v-row>
      <v-col cols="12" md="6">
        <v-list>
          <v-list-subheader>Student Information </v-list-subheader>
          <v-list-item title="Student Name" class="mt-5" subtitle="Sabbir Hasan"></v-list-item>
          <v-list-item title="Tution Location" class="mt-5" subtitle="Mirpur 6, Bangla Bazar, Dhaka"></v-list-item>
        </v-list>
        <v-divider class="mt-5"></v-divider>
        <v-list>
          <v-list-subheader>Others</v-list-subheader>
        </v-list>

        <v-card-text style="padding: 20px 10px;">
          <v-row>
            <v-col cols="12" md="6">
              <v-list-item prepend-icon="mdi-flag-checkered">
                <v-list-item-title>Location</v-list-item-title>
                <v-list-item-subtitle>
                  Mirpur 6, Bangla Bazar, Dhaka
                </v-list-item-subtitle>
              </v-list-item>
            </v-col>
            <v-col cols="12" md="6">
              <v-list-item prepend-icon="mdi-flag-checkered">
                <v-list-item-title>Course</v-list-item-title>
                <v-list-item-subtitle>
                  HSC 2023
                </v-list-item-subtitle>
              </v-list-item>
            </v-col>
            <v-col cols="12" md="6">
              <v-list-item prepend-icon="mdi-briefcase-outline">
                <v-list-item-title>Section </v-list-item-title>
                <v-list-item-subtitle>
                  Science
                </v-list-item-subtitle>
              </v-list-item>
            </v-col>
            <v-col cols="12" md="6">
              <v-list-item prepend-icon="mdi-web-box">
                <v-list-item-title>Version</v-list-item-title>
                <v-list-item-subtitle>
                  English Medium
                </v-list-item-subtitle>
              </v-list-item>
            </v-col>
            <v-col cols="12" md="6">
              <v-list-item prepend-icon="mdi-flag-checkered">
                <v-list-item-title>Student Gender</v-list-item-title>
                <v-list-item-subtitle>
                  Male
                </v-list-item-subtitle>
              </v-list-item>
            </v-col>
            <v-col cols="12" md="6">
              <v-list-item prepend-icon="mdi-briefcase-outline">
                <v-list-item-title>Institute </v-list-item-title>
                <v-list-item-subtitle>
                  Daffodil International University
                </v-list-item-subtitle>
              </v-list-item>
            </v-col>
            <v-col cols="12" md="6">
              <v-list-item prepend-icon="mdi-web-box">
                <v-list-item-title>Salary</v-list-item-title>
                <v-list-item-subtitle>
                  4000
                </v-list-item-subtitle>
              </v-list-item>
            </v-col>

          </v-row>
        </v-card-text>

      </v-col>
      <v-divider vertical></v-divider>
      <v-col cols="12" md="6">
        <v-list>
          <v-list-subheader>Tutors Information </v-list-subheader>
          <v-list-item>
            <v-list-item-title>
              Note
            </v-list-item-title>
            <v-list-item-subtitle>
              <p style="display: flex;">
                Lorem, ipsum dolor sit amet consectetur adipisicing elit. Saepe praesentium animi ratione soluta optio
                esse
                deserunt nostrum. Sint, praesentium amet!
              </p>
            </v-list-item-subtitle>
          </v-list-item>
        </v-list>


        <v-card-text style="padding: 20px 10px;">
          <v-row>
            <v-col cols="12" md="6">
              <v-list-item prepend-icon="mdi-flag-checkered">
                <v-list-item-title>Possible Location</v-list-item-title>
                <v-list-item-subtitle>
                  Mirpur 6 or Nearby
                </v-list-item-subtitle>
              </v-list-item>
            </v-col>
            <v-col cols="12" md="6">
              <v-list-item prepend-icon="mdi-flag-checkered">
                <v-list-item-title>University Type</v-list-item-title>
                <v-list-item-subtitle>
                  Public
                </v-list-item-subtitle>
              </v-list-item>
            </v-col>
            <v-col cols="12" md="6">
              <v-list-item prepend-icon="mdi-briefcase-outline">
                <v-list-item-title>Depertment </v-list-item-title>
                <v-list-item-subtitle>
                  Depertment of Computer Science and Engineering
                </v-list-item-subtitle>
              </v-list-item>
            </v-col>
            <v-col cols="12" md="6">
              <v-list-item prepend-icon="mdi-web-box">
                <v-list-item-title>Version</v-list-item-title>
                <v-list-item-subtitle>
                  English Medium
                </v-list-item-subtitle>
              </v-list-item>
            </v-col>
            <v-col cols="12" md="6">
              <v-list-item prepend-icon="mdi-flag-checkered">
                <v-list-item-title> Gender</v-list-item-title>
                <v-list-item-subtitle>
                  Male
                </v-list-item-subtitle>
              </v-list-item>
            </v-col>
            <v-col cols="12" md="6">
              <v-list-item prepend-icon="mdi-briefcase-outline">
                <v-list-item-title>Minimum Exp </v-list-item-title>
                <v-list-item-subtitle>
                  2 Years
                </v-list-item-subtitle>
              </v-list-item>
            </v-col>

          </v-row>
        </v-card-text>
        <v-card-actions style="display: flex; justify-content: center; align-items: center;">
          <v-btn block rounded="0" size="x-large" color="primary">Apple now</v-btn>
        </v-card-actions>
      </v-col>
    </v-row>
  </div>
</template>

<style scoped></style>
