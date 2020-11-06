<template>
  <v-row justify="center">
    <v-expansion-panels popout>
      <v-expansion-panel
        v-for="(route, id) in routes"
        :key="id"
        style="margin-bottom: 5px"
      >
        <v-expansion-panel-header
          ><row
            style="display: flex;
    justify-content: space-between;"
            ><h1>{{ route.station }}</h1>
            <h1 style="font-family: cursive;">{{ route.dtime }}</h1></row
          ></v-expansion-panel-header
        >
        <v-expansion-panel-content>
          <div
            style="display: flex;
    justify-content: space-around;"
          >
            <div>
              <v-icon large color="green darken-2">
                mdi-map-marker
              </v-icon>
              Address: {{ route.address }}
            </div>
            <div>
              <v-icon large color="green darken-2">
                mdi-clock
              </v-icon>
              Estimated time: {{ route.esttime }}
            </div>
          </div>
          <div
            style="display: flex;
    justify-content: space-around;"
          >
            <div>
              <v-icon large color="green darken-2">
                mdi-routes
              </v-icon>
              Enroute: {{ route.enroute }}
            </div>
            <div>
              <v-icon large color="green darken-2">
                mdi-phone
              </v-icon>
              Phone: {{ route.phone }}
            </div>
          </div>
        </v-expansion-panel-content>
      </v-expansion-panel>
    </v-expansion-panels>
  </v-row>
</template>
<script>
export default {
  data: () => ({
    routes: [
      {
        station: "Faisal Movers",
        dtime: "10:00pm",
        esttime: "12 hrs",
        address: "Band Rd, Kot Kamboh Lahore, Punjab 54000",
        phone: "(042) 111 224 488",
        enroute: "Multan, DGKhan, RJP"
      },
      {
        station: "Daewoo",
        dtime: "10:00pm",
        esttime: "12 hrs",
        address: "Band Rd, Kot Kamboh Lahore, Punjab 54000",
        phone: "(042) 111 224 488",
        enroute: "RJP, DGKhan, Multan"
      },
      {
        station: "Faisal Movers",
        dtime: "10:00pm",
        esttime: "12 hrs",
        address: "Band Rd, Kot Kamboh Lahore, Punjab 54000",
        phone: "(042) 111 224 488",
        enroute: "Multan, DGKhan, RJP"
      },
      {
        station: "Daewoo",
        dtime: "10:00pm",
        esttime: "12 hrs",
        address: "Band Rd, Kot Kamboh Lahore, Punjab 54000",
        phone: "(042) 111 224 488",
        enroute: "RJP, DGKhan, Multan"
      },
      {
        station: "Faisal Movers",
        dtime: "10:00pm",
        esttime: "12 hrs",
        address: "Band Rd, Kot Kamboh Lahore, Punjab 54000",
        phone: "(042) 111 224 488",
        enroute: "Multan, DGKhan, RJP"
      },
      {
        station: "Daewoo",
        dtime: "10:00pm",
        esttime: "12 hrs",
        address: "Band Rd, Kot Kamboh Lahore, Punjab 54000",
        phone: "(042) 111 224 488",
        enroute: "RJP, DGKhan, Multan"
      },
      {
        station: "Faisal Movers",
        dtime: "10:00pm",
        esttime: "12 hrs",
        address: "Band Rd, Kot Kamboh Lahore, Punjab 54000",
        phone: "(042) 111 224 488",
        enroute: "Multan, DGKhan, RJP"
      },
      {
        station: "Daewoo",
        dtime: "10:00pm",
        esttime: "12 hrs",
        address: "Band Rd, Kot Kamboh Lahore, Punjab 54000",
        phone: "(042) 111 224 488",
        enroute: "RJP, DGKhan, Multan"
      },
      {
        station: "Faisal Movers",
        dtime: "10:00pm",
        esttime: "12 hrs",
        address: "Band Rd, Kot Kamboh Lahore, Punjab 54000",
        phone: "(042) 111 224 488",
        enroute: "Multan, DGKhan, RJP"
      },
      {
        station: "Daewoo",
        dtime: "10:00pm",
        esttime: "12 hrs",
        address: "Band Rd, Kot Kamboh Lahore, Punjab 54000",
        phone: "(042) 111 224 488",
        enroute: "RJP, DGKhan, Multan"
      }
    ]
  })
};
</script>
