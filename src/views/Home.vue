<template>
  <div class="home">
    <QuizComponent/>
  </div>
</template>

<script>
// @ is an alias to /src
import QuizComponent from "@/components/QuizComponent.vue";
import "@fortawesome/fontawesome-free/css/all.css";

export default {
  name: "home",
  components: {
    QuizComponent
  }
};
</script>
