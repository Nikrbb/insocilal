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

        <span class="check__descr">Up to 15x more effective than Instagram Bots</span>
      </div>
      <div class="check animation">

      </div>
   </section>
  </div>

</template>

<script>

</script>

<style lang="scss">
  .subtitle {
    &__head {
      font-weight: 600;
      font-size: 36px;
      line-height: 44px;
      margin: 0;
    }
    &__underline {
      display: block;
      height: 4px;
      width: 100%;
      background: linear-gradient(135deg, #00FF5B 0%, #0046DC 100%);
    }
    &__text {
      font-size: 18px;
      line-height: 22px;
      margin: 0;
    }
  }
  .check {
    padding-top: 100px;
    max-width: 600px;
    &__descr {

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
    }

    &__descr {

    }
  }
</style>