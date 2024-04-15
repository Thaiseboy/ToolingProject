<!-- views/HelloWorld.vue -->
<template>
  <div>
    <div class="hello">
      <v-app>
        <v-container>
          <h1>{{ msg }}</h1>
          <v-row>
            <v-col>
              <TweedeTekst />
            </v-col>
          </v-row>
          <DashBoard />
        </v-container>
      </v-app>
    </div>
    <DashBoardInspecties />
  </div>
</template>

<script>
import TweedeTekst from '@/components/tweede-tekst.vue'; 
import DashBoard from '@/components/dash-board.vue'; 
import DashBoardInspecties from '@/components/dash-board-inspecties.vue'; 

export default {
  name: 'HelloWorld',
  components: {
    TweedeTekst,
    DashBoard,
    DashBoardInspecties, 
  },
  props: {
    msg: {
      type: String,
      required: true,
    },
  },
};
</script>

<style scoped>
.hello {
  border: 3px solid black;
  background-color: rgba(0, 170, 162, 1);
}
</style>
