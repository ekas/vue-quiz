<template>
  <div class="container">
    <div class="quiz_header">
      <div class="quiz_quest_icon">
        <img src="../assets/quizImg_1.svg" alt>
      </div>
      <div class="quiz_quest_text">
        <p>Do you party very often?</p>
      </div>
    </div>
    <div class="quiz_choice_container">
      <span class="quiz_choices">
        <span class="choice_option">A</span>
        <span class="choice_text">Yes</span>
        <span></span>
      </span>
      <span class="quiz_choices">
        <span class="choice_option">B</span>
        <span class="choice_text">No</span>
        <span class="choice_selected">
          <i class="fas fa-check-circle"></i>
        </span>
      </span>
    </div>
    <div class="quiz_footer">
      <div class="footer_container">
        <div class="footer_progress_bar_container">
          <div class="footer_progress_bar">
            <div class="footer_progress"></div>
          </div>
        </div>
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
}

/*Header*/
.quiz_header {
  text-align: center;
  /*height: calc(100% - 80px);*/
  width: 100%;
  padding: 100px 0 0;

  .quiz_quest_icon img {
    height: 100px;
  }

  .quiz_quest_text p {
    color: #21232c;
    font-size: 35px;
    font-weight: 600;
    word-spacing: 1.5px;
    letter-spacing: 0.5px;
    line-height: 46px;
  }
}

/* Body */
.quiz_choice_container {
  padding: 50px 0 0;
  text-align: center;

  .quiz_choices {
    background-color: #fff;
    border: solid 1.5px #5861ae;
    letter-spacing: -0.5px;
    padding: 13px 44px 13px 12px;
    color: #21232c;
    width: 125px;
    margin: 0 auto;
    border-radius: 9px;
    font-size: 15px;
    font-weight: 600;
    -webkit-box-shadow: 0px 0px 0px 4px rgba(223, 224, 239, 1);
    -moz-box-shadow: 0px 0px 0px 4px rgba(223, 224, 239, 1);
    box-shadow: 0px 0px 0px 4px rgba(223, 224, 239, 1);
    margin-left: 20px;
    position: relative;
  }
  .choice_option {
    border: solid 1px #c6c9d2;
    color: #c6c9d2;
    padding: 2px 5px;
    border-radius: 3px;
    margin-right: 5px;
  }

  .choice_selected {
    position: absolute;
    right: 10px;
    top: 11px;
    font-size: 20px;
    color: #5861ae;
  }
}

/* Footer */

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

  .footer_container {
    padding: 10px 20px;

    .footer_progress_bar_container {
      width: 500px;
      padding: 24px 0;
      float: left;

      .footer_progress_bar {
        background-color: #ecedf5;
        width: 100%;
        height: 14px;
        border-radius: 7px;
        position: relative;
      }

      .footer_progress {
        position: absolute;
        background-color: #5861ae;
        width: 50%;
        height: 14px;
        border-radius: 7px;
      }
    }
  }

  .footer_buttons {
    margin-top: 11px;
    float: right;

    button {
      padding: 10px 15px;
      border: solid 1px #dfe1ef;
      background-color: #fff;
      margin: 0;

      .btn_prev {
        border-top-left-radius: 5px;
        border-bottom-left-radius: 5px;
      }

      .btn_next {
        border-top-right-radius: 5px;
        border-bottom-right-radius: 5px;
      }
      i {
        color: #8d94a4;
        font-size: 20px;
      }
    }
  }
}
</style>
