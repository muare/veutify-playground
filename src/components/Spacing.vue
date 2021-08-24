<template>
  <div>
    <h3 class="ma-sm-5">Spacing</h3>
    <v-card class="mt-5 mb-8">
        <v-card-text>
            <v-container class="spacing-playground py-0 px-2" fluid>
                <v-row>
                    <v-col cols="12"  class="d-flex align-center">
                        <v-select v-model="paddingDirection" :items="paddingDirections" label="Padding" class="pr-2">
                            <template v-slot:prepend> 
                                <strong class="text--primary">p</strong>
                            </template>
                            <template v-slot:append-outer> 
                                <strong class="text--primary">-</strong>
                            </template>
                        </v-select>
                        <v-select v-model="paddingSize" :items="paddingSizes.slice(1)" label="Size">
                        </v-select>
                    </v-col>

                    <v-col cols="12"  class="d-flex align-center">
                        <v-select v-model="marginDirection" :items="marginDirections" label="Margin" class="pr-2">
                            <template v-slot:prepend> 
                                <strong class="text--primary">m</strong>
                            </template>
                            <template v-slot:append-outer> 
                                <strong class="text--primary">-</strong>
                            </template>
                        </v-select>
                        <v-select v-model="marginSize" :items="marginSizes.slice(1)" label="Size">
                        </v-select>
                    </v-col>

                    <v-col>
                        <v-card :class="computedMargin" class="elevation-4">
                            <div :class="computedPadding" class="light-green lighten-3">
                                <div class="white text-center">
                                    {{playgroundText}}                                    
                                </div>
                            </div>
                        </v-card>
                    </v-col>
                </v-row>
            </v-container>
        </v-card-text>
    </v-card>
  </div>
</template>

<script>
export default {
    data() {
        return {
            paddingDirections: ['t', 'b', 'l', 'r', 's', 'e', 'x', 'y', 'a'],
            paddingSizes: ['auto', '0', '1', '2', '3', '4', '5', '6', '7', '8', '9', '10', '11', '12'],
            marginDirections: ['t', 'b', 'l', 'r', 's', 'e', 'x', 'y', 'a'],
            marginSizes: ['auto', '0', '1', '2', '3', '4', '5', '6', '7', '8', '9', '10', '11', '12'],
            paddingDirection: 'a',
            paddingSize: '2',
            marginDirection: 'a',
            marginSize: '2',
            playgroundText: 'Use the controls abouve to try out the different spacing helpers'
        }
    },
    computed: {
        computedPadding() {
            return `p${this.paddingDirection}-${this.paddingSize}`
        },
        computedMargin() {
            return `p${this.marginDirection}-${this.marginSize}`
        }
    }
}
</script>


<style scoped>
.spacing-playground .v-select .v-input__prepend-outer, .spacing-playground .v-select .v-input__append-outer{
  margin-top: 0.55rem;
  margin-right: 0.2rem;
}
</style>