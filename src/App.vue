<template>
  <v-app>
    <v-content>
      <v-container>
        <v-row>
          <v-col cols="12">
            <v-row class="mb-12">
              <v-col cols="12">
                <h1 class="mt-5 mb-5">Playground</h1>
                <v-divider />
              </v-col>
            </v-row>
            <v-row class="mb-12">
              <v-col cols="12">
                <Typography />
                <v-divider />
              </v-col>
            </v-row>
            <v-row  class="mb-12">
              <v-col cols="12">
                <Spacing />
                <v-divider />
              </v-col>
            </v-row>
            <v-row class="mb-12">
              <v-col cols="12">
                <Button />
                <v-divider />
              </v-col>
            </v-row>
            <v-row class="mb-12">
              <v-col cols="12">
                <Menu />
                <v-divider />
              </v-col>
            </v-row>
            <v-row class="mb-12">
              <v-col cols="12">
                <Grid />
                <v-divider />
              </v-col>
            </v-row>
            <v-row class="mb-12">
              <v-col cols="12">
                <Card />
                <v-divider />
              </v-col>
            </v-row>
          </v-col>
        </v-row>
      </v-container>
    </v-content>
  </v-app>
</template>

<script>
import Typography from "./components/Typography.vue";
import Spacing from "./components/Spacing.vue";
import Button from "./components/Button.vue";
import Menu from "./components/Menu.vue";
import Grid from "./components/Grid.vue";
import Card from "./components/Card.vue";

export default {
  name: "App",

  components: {
    Typography,
    Spacing,
    Button,
    Menu,
    Grid,
    Card,
  },

  data: () => ({
    //
  }),
};
</script>
