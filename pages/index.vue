<template>
  <v-row justify="center" align="center">
    <v-col cols="12" sm="8" md="6">
      <div class="text-center">
        <!-- <logo />
        <vuetify-logo /> -->
      </div>
      <v-card>
        <v-card-title class="headline">
          Welcome to our community site.
        </v-card-title>
        <v-card-text>
          <p>発足：2019年11月より</p>
          <p>運営方法：Slack</p>
          <p>メンバー：9名</p>
          <p>
            <a
              href="https://naruhiro-portfolio.firebaseapp.com/"
              target="_blank"
              rel="noopener noreferrer"
              title="my_site"
            >
              運営者サイト
            </a>
          </p>
          <div class="text-xs-right">
            <em><small>&mdash; Increment</small></em>
          </div>
          <hr class="my-3">
          <!-- <a
            href="https://nuxtjs.org/"
            target="_blank"
            rel="noopener noreferrer"
          >
            Nuxt Documentation
          </a> -->
          <br>
          <!-- <a
            href="https://github.com/nuxt/nuxt.js"
            target="_blank"
            rel="noopener noreferrer"
          >
            Nuxt GitHub
          </a> -->
        </v-card-text>
        <v-card-actions>
          <v-spacer />
          <v-btn
            color="primary"
            nuxt
            to="/member"
          >
            Continue
          </v-btn>
        </v-card-actions>
      </v-card>
    </v-col>
  </v-row>
</template>

<script>
// import Logo from '~/components/Logo.vue'
// import VuetifyLogo from '~/components/VuetifyLogo.vue'

export default {
  components: {
  }
}
</script>
