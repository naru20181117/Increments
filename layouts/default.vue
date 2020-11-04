<template>
  <v-app light>
    <v-card class="overflow-hidden">
      <v-navigation-drawer
        v-model="drawer"
        app
      >
        <v-list>
          <v-list-item
            v-for="(item, i) in items"
            :key="i"
            :to="item.to"
            router
            exact
          >
            <v-list-item-action>
              <v-icon>{{ item.icon }}</v-icon>
            </v-list-item-action>
            <v-list-item-content>
              <v-list-item-title v-text="item.title" />
            </v-list-item-content>
          </v-list-item>
        </v-list>
      </v-navigation-drawer>
      <v-app-bar
        app
        absolute
        color="white"
        elevate-on-scroll
      >
        <v-app-bar-nav-icon @click.stop="drawer = !drawer" />
        <v-toolbar-title v-text="title" />
        <v-spacer />
      </v-app-bar>
      <!-- <v-sheet
        id="scrolling-techniques-7"
        class="overflow-y-auto"
        max-height="900"
      > -->
      <v-main>
        <!-- <v-container style="max-height: 1500px;"> -->
        <v-parallax src="https://cdn.vuetifyjs.com/images/parallax/material.jpg" />
        <nuxt />
        <!-- </v-container> -->
      </v-main>
      <!-- </v-sheet> -->
    </v-card>
    <v-footer
      :absolute="true"
      app
    >
      <span>&copy; {{ new Date().getFullYear() }}</span>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  data () {
    return {
      drawer: false,
      items: [
        {
          icon: 'mdi-apps',
          title: 'Home',
          to: '/'
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'Member',
          to: '/member'
        }
      ],
      title: 'Increment'
    }
  }
}
</script>
