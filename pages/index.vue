<script>
export default {
  data: () => ({
    dialog: false,
    barlinks: [
      {
        title: 'Home',
        disabled: false,
        href: 'breadcrumbs_dashboard',
      },
      {
        title: 'Jobs',
        disabled: false,
        href: 'breadcrumbs_link_1',
      },
      {
        title: 'Applied Jobs',
        disabled: true,
        href: 'breadcrumbs_link_2',
      },
    ],

  }),
}
</script>

<template>
  <v-container style="max-width: 1500px">
    <v-layout>
      <v-main style="height: 500px;">
        <v-breadcrumbs :items="barlinks" divider="/"></v-breadcrumbs>
        <v-row style="margin: 10px 4px">
          <v-col cols="12" sm="6" md="4">
            <v-card>
              <v-card-title>HSC 2023</v-card-title>
              <v-card-subtitle>Mirpur 6 </v-card-subtitle>
              <v-card-text style="padding: 20px 10px;">
                <v-row>

                  <v-list style=" display: flex;flex-wrap: wrap;gap: 10px;">
                    <v-list-item prepend-icon="mdi-flag-checkered">

                      <v-list-item-title>HSC</v-list-item-title>
                      <v-list-item-subtitle>Class</v-list-item-subtitle>

                    </v-list-item>
                    <v-list-item prepend-icon="mdi-briefcase-outline">

                      <v-list-item-title>Science </v-list-item-title>
                      <v-list-item-subtitle>Section</v-list-item-subtitle>

                    </v-list-item>

                    <v-list-item prepend-icon="mdi-web-box">

                      <v-list-item-title>English</v-list-item-title>
                      <v-list-item-subtitle>Version</v-list-item-subtitle>

                    </v-list-item>

                    <v-list-item prepend-icon="mdi-cash-multiple">

                      <v-list-item-title>4000</v-list-item-title>
                      <v-list-item-subtitle>Salary</v-list-item-subtitle>

                    </v-list-item>
                    <v-list-item prepend-icon="mdi-book-multiple-outline">

                      <v-list-item-title>Banhla, English, Math</v-list-item-title>
                      <v-list-item-subtitle>Subjects</v-list-item-subtitle>

                    </v-list-item>
                  </v-list>

                </v-row>
              </v-card-text>
              <v-card-actions style="display: flex; justify-content: end; align-items: center;">
                <v-btn border class="text-none" color="primary" prepend-icon="mdi-check" variant="text">
                  Interested
                </v-btn>

                <v-dialog v-model="dialog" fullscreen :scrim="false" transition="dialog-bottom-transition">
                  <template v-slot:activator="{ props }">
                    <v-btn color="primary" variant="tonal" dark v-bind="props">
                      View Details
                    </v-btn>
                  </template>
                  <v-card>
                    <v-toolbar dark color="primary">
                      <v-btn icon dark @click="dialog = false">
                        <v-icon>mdi-close</v-icon>
                      </v-btn>
                      <v-toolbar-title>Job Details</v-toolbar-title>
                      <v-spacer></v-spacer>
                      <v-toolbar-items>
                        <v-btn variant="text" @click="dialog = false">
                          Cancle
                        </v-btn>
                      </v-toolbar-items>
                    </v-toolbar>
                    <JobDetail />
                  </v-card>
                </v-dialog>
              </v-card-actions>
            </v-card>
          </v-col>
        </v-row>
      </v-main>
    </v-layout>
  </v-container>
</template>
<style scoped>
.dialog-bottom-transition-enter-active,
.dialog-bottom-transition-leave-active {
  transition: transform .2s ease-in-out;
}
</style>
