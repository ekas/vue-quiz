<template>
  <div class="container">
    <div class="quiz_header">
      <div class="quiz_quest_icon">
        <i class="fab fa-accessible-icon"></i>
      </div>
      <div class="quiz_quest_header">
        <h1>Do you smoke cigarettes on Daily basis?</h1>
      </div>
    </div>
    <div class="quiz_choices"></div>
    <div class="quiz_footer">
      <div class="footer_container">
        <div class="footer_progress_bar"></div>
        <div class="footer_buttons">
          <button class="btn_prev">
            <i class="fas fa-angle-left"></i>
          </button>
          <button class="btn_next">
            <i class="fas fa-angle-right"></i>
          </button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "QuizComponent"
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.container {
  background-color: #f7f8fc;
  height: 100vh;
  width: 100vw;
  overflow: hidden;
}
.quiz_header {
  text-align: center;
  height: calc(100% - 80px);
  width: 100%;
  overflow-y: scroll;
}
.quiz_footer {
  width: 100%;
  height: 80px;
  background-color: #fff;
  border-top: solid 2px #dfe1ef;
  position: fixed;
  bottom: 0;
  -webkit-box-shadow: -1px -6px 9px -3px rgba(223, 225, 239, 0.85);
  -moz-box-shadow: -1px -6px 9px -3px rgba(223, 225, 239, 0.85);
  box-shadow: -1px -6px 9px -3px rgba(223, 225, 239, 0.85);
}

/* Footer */
.footer_container {
  padding: 10px 20px;

  .footer_buttons {
    margin-top: 11px;
    float: right;
  }
  .footer_buttons button {
    padding: 10px 15px;
    border: solid 1px #dfe1ef;
    background-color: #fff;
  }
  .footer_buttons button i {
    color: #8d94a4;
    font-size: 20px;
  }
  .btn_prev {
    border-top-left-radius: 5px;
    border-bottom-left-radius: 5px;
  }
  .btn_next {
    border-top-right-radius: 5px;
    border-bottom-right-radius: 5px;
  }
}
</style>
