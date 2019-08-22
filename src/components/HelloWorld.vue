<template>
  <v-container>
    <v-layout
      text-center
      wrap
    >
      <v-flex xs12>
        <v-img
          :src="require('../assets/GDOT_logo.png')"
          class="my-3"
          contain
          height="200"
        ></v-img>
      </v-flex>

      <v-flex mb-4>
        <h1 class="display-2 mb-3">
          Welcome to the Meeting Documents Site for GDOT's </br>Statewide Transit Plan (SWTRP)
        </h1>
        <p class="subheading font-weight-regular">
          For more information about the SWTRP
          <br>please visit
          <a href="http://www.dot.ga.gov/InvestSmart/Transit/Pages/TransitPlan.aspx" target="_blank">SWTRP's page on GDOT's website</a>
        </p>
      </v-flex>

      <v-flex
        xs12
        mb-5
      >
        <h2 class="headline font-weight-bold mb-3">Documents</h2>

        <v-layout justify-center>
          <a
            v-for="(doc, i) in documents"
            :key="i"
            :href="doc.href"
            class="subheading mx-3"
            target="_blank"
          >
            {{ doc.text }}
          </a>
        </v-layout>
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
export default {
  data: () => ({
    documents: [
      {
        text: 'SWTRP Placeholder Doc 1',
        href: 'https://firebasestorage.googleapis.com/v0/b/swtrp-9fda0.appspot.com/o/SWTRP_Placeholder.pdf?alt=media&token=7c462c0b-5677-401b-b525-f93840e8aebd',
      },
      {
        text: 'SWTRP Placeholder Doc 2',
        href: 'https://firebasestorage.googleapis.com/v0/b/swtrp-9fda0.appspot.com/o/SWTRP_Placeholder.pdf?alt=media&token=7c462c0b-5677-401b-b525-f93840e8aebd',
      },
      {
        text: 'SWTRP Placeholder Doc 3',
        href: 'https://firebasestorage.googleapis.com/v0/b/swtrp-9fda0.appspot.com/o/SWTRP_Placeholder.pdf?alt=media&token=7c462c0b-5677-401b-b525-f93840e8aebd',
      },
    ],
  }),
};
</script>
