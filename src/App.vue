<template>
  <v-app>
    <v-app-bar app>
      <v-toolbar-title class="headline text-uppercase">
        <span>GDOT</span>
        <span class="font-weight-light"> Statewide Transit Plan Documents</span>
      </v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn
        text
        href="http://www.dot.ga.gov/InvestSmart/Transit/Pages/TransitPlan.aspx"
        target="_blank"
      >
        <span class="mr-2">Main site</span>
      </v-btn>
    </v-app-bar>

    <v-content>
      <HelloWorld/>
    </v-content>
  </v-app>
</template>

<script>
import HelloWorld from './components/HelloWorld';

export default {
  name: 'App',
  components: {
    HelloWorld,
  },
  data: () => ({
    //
  }),
};
</script>
