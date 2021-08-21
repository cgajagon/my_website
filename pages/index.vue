<template>
  <section id="intro">
    <v-row class="white--text mx-auto py-12" justify="center">
      <v-col class="white--text text-center" cols="12" tag="h1">
        <span
          :class="[$vuetify.breakpoint.smAndDown ? 'display-1' : 'display-2']"
          class="font-weight-black"
        >
          CARLOS GAJARDO GONZALEZ
        </span>

        <br />

        <span class="font-weight-light">
            Engineer | Maker
        </span>

      </v-col>
    </v-row>
    <v-row>
      <v-col class="text-center">
        <blockquote class="blockquote">
          &#8220;First, solve the problem. Then, write the code.&#8221;
          <footer>
            <small>
              <em>&mdash;John Johnson</em>
            </small>
          </footer>
        </blockquote>
      </v-col>
    </v-row>
    <v-row justify="center">
      <v-col class="white--text text-center" cols="10" tag="icons">
        <v-card class="py-12 px-4" color="rgba(3, 37, 76, 0.50)">
          <v-row>
            <v-col
              v-for="({ icon, link }, i) in features"
              :key="i"
            >
              <v-btn x-large v-bind:href="link" fab outlined>
                <v-icon v-text="icon" x-large> </v-icon
              ></v-btn>
            </v-col>
          </v-row>
        </v-card>
      </v-col>
    </v-row>
  </section>
</template>

<script>
export default {
  data() {
    return {
      features: [
        {
          icon: "mdi-email",
          title: "Vibrant Community",
          link: "mailto:cgajagon@gmail.com"
        },
        {
          icon: "mdi-linkedin",
          title: "Frequent Updates",
          link: "https://www.linkedin.com/in/carlos-gajardo-gonz%C3%A1lez-product-development-it/"
        },
        {
          icon: "mdi-github",
          title: "Long-term Support",
          link: "https://github.com/cgajagon"
        }
      ]
    };
  }
};
</script>