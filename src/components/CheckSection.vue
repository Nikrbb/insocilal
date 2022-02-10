<template>
  <div class="container">
   <section class="check">

      <div class="check__descr">
        <div class="subtitle check__subtitle">
          <h2 class="subtitle__head">Check your growth</h2>
          <span class="subtitle__underline"></span>
          <p class="subtitle__text">See your account after 30 days with Insocial </p>
        </div>
        <div class="check__find-field">
          <div class="check__find-logo">
            <img class="check__find-img" src="../assets/insta.png" alt="instagram">
          </div>
          <input class="check__input" placeholder="Enter Instagram account..." type="text">
          <button class="check__btn">PREVIEW GROWTH</button>
        </div>

        <span class="check__text">Up to 15x more effective than Instagram Bots</span>
      </div>
      <div class="check__animation">
        <div class="check__phone">
          <img src="../assets/check/phone_check.png" alt="">
        </div>
        <div class="check__robot">
          <img src="../assets/check/robot_check.png" alt="">
        </div>
        <div class="check__circle">
          <img src="../assets/check/ellipce_check.png" alt="">
        </div>
      </div>
   </section>
  </div>

</template>

<script>

</script>

<style lang="scss">
  .check {
    display: flex;
    margin-top: 150px;
    padding-bottom: 43px;

    &__descr {
      padding-top: 100px;
      text-align: left;
      max-width: 600px;
      width: 100%;
    }

    &__subtitle {
      max-width: 400px;
    }

    &__find-field {
      display: flex;
      align-items: center;
      width: 100%;
      margin-top: 40px;
      border: 2px solid #07166C;
      border-radius: 16px;
    }
    &__find-logo {
      margin-left: 24px;
    }
    &__find-img {
      width: 32px;
      height: 32px;
    }

    &__input {
      border: none;
      margin-left: 24px;
      width: 100%;
      padding: 24px 0;
    }

    &__btn {
      border-top-right-radius: 16px;
      border-bottom-right-radius: 16px;
      padding: 24px;
      border: none;
      border-left: 2px solid #07166C;;
      white-space: nowrap;
      background-color: #38D89A;
      font-size: 18px;
      line-height: 22px;
      font-weight: 700;
    }

    &__text {
      text-align: left;
      display: inline-block;
      margin-top: 14px;
    }

    &__animation {
      position: relative;
      max-width: 600px;
      width: 100%;
      height: 570px;
    }

    &__phone {
      position: absolute;
      top: 0;
      left: 50%;
      transform: translateX(-50%);
      z-index: 2;
    }

    &__robot {
      position: absolute;
      top: -7%;
      left: 52%;
      transform: translateX(-30%);
      z-index: 3;
    }

    &__circle {
      position: absolute;
      bottom: 0;
      left: 50%;
      transform: translateX(-50%);
      z-index: 1;
    }
  }
</style>