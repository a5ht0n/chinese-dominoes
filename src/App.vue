<template>
  <v-app>
    <v-app-bar
      app
      color="accent"
      dark
    >
   <div class="d-flex align-center">
        <div>Chinese Dominoes</div>
    </div>
    </v-app-bar>

    <v-main>
      <ContestantSignUp/>
    </v-main>
  </v-app>
</template>

<script>
import ContestantSignUp from './components/ContestantSignUp';

export default {
  name: 'App',

  components: {
    ContestantSignUp
  },

  data: () => ({
    //
  }),
};
</script>
