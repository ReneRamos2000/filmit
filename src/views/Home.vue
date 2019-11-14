<template>
  <div class="home mb-5">
    <div mx-5>
      <v-row>
        <v-column v-for="card in cards" :key="card.title">
          <v-card outlined class="ma-5">
            <v-img
              height="200"
              width="200"
              :src="card.img"
            ></v-img>
            <v-card-title class="text-center">
              {{card.title}}
            </v-card-title>
          </v-card>
        </v-column>
      </v-row>
      <v-row>
        <Form></Form>
      </v-row>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import spidermanposter from '@/assets/spiderman.jpeg';
import interstellarposter from '@/assets/interstellar.jpeg';
import jokerposter from '@/assets/thejoker.jpeg';
import avengersposter from '@/assets/avengers.jpeg';
import Form from '@/components/Form.vue';

export default {
  name: 'home',
  components: {
    Form,
  },
  data: () => ({
    cards: [
      { title: 'Interstellar', img: interstellarposter },
      { title: 'Spider Man', img: spidermanposter },
      { title: 'The Avengers', img: avengersposter },
      { title: 'The Joker', img: jokerposter },
    ],
  }),
};
</script>
