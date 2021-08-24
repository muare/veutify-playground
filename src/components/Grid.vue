<template>
  <div>
    <h3>Grid</h3>
    <v-card class="mt-5 mb-8">
      <v-card-text>
        <v-container>
          <v-row no-gutters>
            <v-col cols="12"> <v-card outlined tile> Column </v-card> </v-col>
          </v-row>
          <v-row no-gutters justify="start">
            <v-col cols="4"> <v-card outlined tile> Column </v-card> </v-col>
            <v-col cols="4"><v-card outlined tile> Column </v-card></v-col>
          </v-row>
        </v-container>
      </v-card-text>
    </v-card>
  </div>
</template>