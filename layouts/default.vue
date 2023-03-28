
<template>
  <div>
    <v-app>
      <v-app-bar color="primary" prominent>
        <v-app-bar-nav-icon variant="text" @click.stop="drawer = !drawer"></v-app-bar-nav-icon>
        <v-toolbar-title>Asif Ekbal</v-toolbar-title>
        <v-spacer></v-spacer>
        <v-btn variant="text" icon="mdi-magnify"></v-btn>
        <v-btn variant="text" icon="mdi-filter"></v-btn>
        <v-menu v-model="menu" :close-on-content-click="false" location="end">
          <template v-slot:activator="{ props }">
            <v-btn v-bind="props" variant="text" icon="mdi-dots-vertical">
            </v-btn>
          </template>
          <v-card min-width="300">
            <v-list>
              <v-list-item prepend-avatar="https://cdn.vuetifyjs.com/images/john.jpg" title="Asif Ekbal"
                subtitle="No name person">
                <template v-slot:append>
                  <v-btn variant="text"
                    :icon='pro ? icon = "mdi-check-decagram" : icon = "mdi-check-decagram-outline"'></v-btn>
                </template>
              </v-list-item>
            </v-list>
            <v-divider></v-divider>
            <v-list>
              <v-list-item prepend-icon="mdi-account">
                Profile
              </v-list-item>
              <v-list-item prepend-icon="mdi-logout">
                Logout
              </v-list-item>
            </v-list>
            <v-card-actions>
              <v-spacer></v-spacer>
              <v-btn variant="text" @click="menu = false">
                Close
              </v-btn>
            </v-card-actions>
          </v-card>
        </v-menu>
      </v-app-bar>
      <v-navigation-drawer v-model="drawer" location="left" temporary>
        <v-list v-for="i in items">
          <v-list-item :prepend-icon="i.icon" :title="i.title" :value="i.value" :to="i.link"></v-list-item>
        </v-list>
      </v-navigation-drawer>
      <slot />
    </v-app>
  </div>
</template>
<script >
export default {

  data: () => ({
    drawer: false,
    group: null,
    items: [
      {
        title: 'Profile',
        value: 'profile',
        icon: 'mdi-account',
        link: '/profile',
      },
      {
        title: 'Jobs',
        value: 'jobs',
        icon: 'mdi-briefcase',
        link: '/',
      },
      {
        title: 'Applied Jobs',
        value: 'applied',
        icon: 'mdi-briefcase-check',
      },
      {
        title: 'Settings',
        value: 'Settings',
        icon: 'mdi-cog',
      },
    ],
    pro: true,
    menu: false,
    message: false,
    hints: true,
  }),
  watch: {
    group() {
      this.drawer = false
    },
  },
}
</script>

<style scoped></style>
