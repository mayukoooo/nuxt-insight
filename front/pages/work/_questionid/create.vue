<template>
  <v-container fluid>
    <v-row>
      <v-col cols="12" md="12">
        <!-- <v-text v-model="$route.params.questionid">{{ questions[$route.params.questionid].text }}</v-text> -->
        {{ questions[$route.params.questionid].text }}
        <v-textarea solo v-model="answer" name="input-7-4" label="入力欄" required></v-textarea>
      </v-col>
    </v-row>
    <v-row justify="space-around">
      <NuxtLink to="/"><v-btn color="#FFAB91">もどる</v-btn></NuxtLink>
      <v-btn @click.prevent="addAnswer" color="#FFAB91">
        つぎへ
      </v-btn>
    </v-row>
  </v-container>
</template>

<script>
import axios from "@/plugins/axios"; 

export default {
  async asyncData({ $axios }) {
    const questions = await $axios.$get(
      "http://localhost:3000/v1/questions"
    );
    return { questions };
  },
  data() {
    return {
      answer: [],
    };
  },
  methods: {
    async addAnswer(answer) {
      await axios.post("http://localhost:3000/v1/answers", { answer }); 
      // this.answer.push({
      //   answer,
      // });
      this.$router.push("/work/1/create");
    },
  },
};
</script>

<style>

</style>