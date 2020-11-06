<template>
  <div>
    <v-card elevation="10" light outlined tile>
      <v-row style="margin: 0px;">
        <v-col>
          From
          <v-autocomplete
            v-model="from"
            style="max-width: 70%;"
            :items="cities"
            auto-select-first
            clearable
          ></v-autocomplete>
        </v-col>
        <v-col>
          To
          <v-autocomplete
            v-model="to"
            style="max-width: 70%;"
            :items="cities"
            auto-select-first
            clearable
          ></v-autocomplete>
        </v-col>
      </v-row>
    </v-card>
    <v-card elevation="10" light outlined tile style="margin-top: 10px">
      <TTPanel v-if="(from !== null) & (to !== null)" />
    </v-card>
  </div>
</template>

<script>
import TTPanel from "../components/timetablepanel";
export default {
  components: {
    TTPanel
  },
  data: () => ({
    from: null,
    to: null,
    cities: ["Lahore", "Karachi", "Rajanpur"]
  })
};
</script>

<style scoped></style>
