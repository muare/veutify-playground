<template>
  <div>
    <h3 class="ma-5">Button</h3>
    <v-card class="mt-5 mb-8">
      <v-card-text>
        <v-row>
          <v-col cols="12">
            <v-btn icon color="error">
              <v-icon>mdi-pencil</v-icon>
            </v-btn>
          </v-col>
        </v-row>
        <v-row>
          <v-col cols="12">
            <v-btn color="red white--text"> Normal </v-btn>
          </v-col>
        </v-row>
        <v-row>
          <v-col cols="12">
            <v-btn tile outlined color="success">
              <v-icon left>mdi-pencil</v-icon>Edit
            </v-btn>
          </v-col>
        </v-row>
        <v-row>
          <v-col cols="12">
            <v-btn text icon color="pink">
              <v-icon>mdi-heart</v-icon>
            </v-btn>
            <v-btn text icon color="deep-orange">
              <v-icon>mdi-thumb-up</v-icon>
            </v-btn>
          </v-col>
        </v-row>
        <v-row>
          <v-col cols="12">
            <v-btn class="mx-2" fab dark color="indigo">
              <v-icon>mdi-plus</v-icon>
            </v-btn>
          </v-col>
        </v-row>        
      </v-card-text>
    </v-card>
  </div>
</template>