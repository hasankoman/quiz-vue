<template>
  <main
    id="test"
    class="d-flex justify-content-center align-items-center mt-5 w-50 mx-auto h-75 my-auto"
  >
    <div class="w-100">
      <ul class="d-flex flex-column gap-3 w-100">
        <li v-for="answer in questions[onIndex].answers" class="mx-0">
          <button
            class="btn btn-outline-info w-100 py-3"
            :class="{
              active: activeAnswer === answer,
              'opacity-75': activeAnswer !== answer
            }"
            @click="activeAnswer = answer"
          >
            {{ answer }}
          </button>
        </li>
        <button
          @click="activeAnswer = 0"
          class="btn btn-outline-info w-100 py-3 "
          :class="{
            active: activeAnswer === 0,
            'opacity-75': activeAnswer !== 0
          }"
        >
          Belirtmek İstemiyorum
        </button>
      </ul>
      <div class="w-100 d-flex flex-row gap-2 mt-5">
        <button
          class=" btn btn-danger py-3 w-50"
          :class="{ 'd-none': onIndex === 0 }"
          @click="prevQuestion"
        >
          Önceki
        </button>
        <button
          class=" btn btn-danger py-3 w-50"
          :class="{ disabled: activeAnswer === null, 'w-100': onIndex === 0 }"
          @click="nextQuestion"
        >
          {{ onIndex === questions.length - 1 ? "Tamamla" : "Devam Et" }}
        </button>
      </div>
    </div>
  </main>
</template>

<script>
import questions from "../database/questions.json";

export default {
  name: "header",
  data() {
    return {
      questions: questions.questions,
      onIndex: 0,
      activeAnswer: null,
      lastQuestion: false,
      userAnswers: []
    };
  },
  methods: {
    nextQuestion() {
      if (this.onIndex === this.questions.length - 1) {
        alert("Test Bitti");
      } else {
        this.userAnswers[this.onIndex] = this.activeAnswer;
        this.onIndex++;
        this.activeAnswer = this.userAnswers[this.onIndex];
        if (!this.userAnswers[this.onIndex]) {
          this.activeAnswer = null;
        }
      }
    },
    prevQuestion() {
      this.activeAnswer = this.userAnswers[this.onIndex - 1];
      this.onIndex--;
      console.log(this.userAnswers);
    }
  }
};
</script>

<style></style>
