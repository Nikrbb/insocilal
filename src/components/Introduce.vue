<template>
  <section class="introduce">
    <div class="container">
      <div class="introduce__descr">
        <h1 class="introduce__title">MARKETING TOOLKIT <br> FOR INSTAGRAM</h1>
        <p class="introduce__text">Become Instagram-famous and skyrocket sales by using pro tools.
          These must-have solutions will help you attract fans, engage with сustomers,
          сurate content, and grow revenue.</p>
        <main-button>
          <a class="introduce__link" href="#">CHECK YOUR GROWTH</a>
        </main-button>
      </div>
      <div class="introduce__animation">
        <ul class="introduce__item-list">
          <li class="introduce__item introduce__item--1"><img class="introduce__item-img" src="../assets/social-icons/active_member.png" alt="social component"></li>
          <li class="introduce__item introduce__item--2"><img class="introduce__item-img" src="../assets/social-icons/active_growth.png" alt="social component"></li>
          <li class="introduce__item introduce__item--3"><img class="introduce__item-img" src="../assets/social-icons/active_auto_promo.png" alt="social component"></li>
          <li class="introduce__item introduce__item--4"><img class="introduce__item-img" src="../assets/social-icons/active_posting_icon.png" alt="social component"></li>
          <li class="introduce__item introduce__item--5"><img class="introduce__item-img" src="../assets/social-icons/active_messages_icon.png" alt="social component"></li>
          <li class="introduce__item introduce__item--6"><img class="introduce__item-img" src="../assets/social-icons/active_liking_icon.png" alt="social component"></li>
          <li class="introduce__item introduce__item--7"><img class="introduce__item-img" src="../assets/social-icons/active_influence_icon.png" alt="social component"></li>
          <li class="introduce__item introduce__item--8"><img class="introduce__item-img" src="../assets/social-icons/active_hashtag_icon.png" alt="social component"></li>
          <li class="introduce__item introduce__item--9"><img class="introduce__item-img" src="../assets/social-icons/active_comment_icon.png" alt="social component"></li>
          <li class="introduce__item introduce__item--10"><img class="introduce__item-img" src="../assets/social-icons/active_posting_icon.png" alt="social component"></li>
          <li class="introduce__item introduce__item--11"><img class="introduce__item-img" src="../assets/social-icons/active_growth.png" alt="social component"></li>
          <li class="introduce__item introduce__item--12"><img class="introduce__item-img" src="../assets/social-icons/active_auto_promo.png" alt="social component"></li>
        </ul>
        <div class="introduce__main-img">
          <img class="introduce__img-body" src="../assets/introduce/robot-main/body.png" alt="robot-body">
          <img class="introduce__img-hand1" src="../assets/introduce/robot-main/hand1.png" alt="robot-hand">
          <img class="introduce__img-hand2" src="../assets/introduce/robot-main/hand2.png" alt="robot-hand">
          <img class="introduce__img-headlight" src="../assets/introduce/robot-main/headlight.png" alt="robot-headlight">
          <img class="introduce__img-ellipse" src="../assets/introduce/robot-main/ellipse.png" alt="robot-ellipse">
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import MainButton from "@/components/MainButton";
export default {
  name: 'Introduce',
  components: {
    MainButton
  }

}

</script>

<style lang="scss">
  .introduce {
    background-color: #fff;
    background-image: url("../assets/introduce/introduce_backgroung.png");
    background-repeat: no-repeat;
    background-position: top;
    padding-bottom: 100px;

    .container {
      display: flex;
    }
    &__descr {
      max-width: 580px;
      text-align: left;
    }

    &__title {
      font-size: 36px;
      line-height: 44px;
      font-weight: 600;
      padding-top: 60px;
      margin: 0;
      color: #F8F8F8;
    }

    &__text {
      font-size: 24px;
      line-height: 29px;
      margin-top: 60px;
    }

    &__link {
      display: inline-block;
      margin-left: 68px;
      font-weight: bold;
      font-size: 18px;
      line-height: 22px;
      color: #07166C;
      &::after {
        content: "";
        display: block;
        height: 2px;
        width: 100%;
        background: linear-gradient(135deg, #00FF5B 0%, #0046DC 100%);
      }
    }

    &__animation {
      width: 100%;
      max-width: 620px;
      position: relative;
    }

    &__item-list {
      display: flex;
      list-style: none;
      padding: 0;
      position: relative;
      height: 100%;
    }
    &__item {
      position: absolute;
      background-color: #FFF;
      border-radius: 50%;
      width: 82px;
      height: 82px;
      display: flex;
      justify-content: center;
      align-items: center;
    }

    &__item--1 {
      top: 0;
      left: 50%;
    }
    &__item--2 {
      top: 10%;
      left: 30%;
    }
    &__item--3 {
      top: 32%;
      left: 15%;
    }
    &__item--4 {
      top: 60%;
      left: 5%;
    }
    &__item--5 {
      top: 88%;
      left: 15%;
    }
    &__item--6 {
      top: 115%;
      left: 30%;
    }

    &__item--7 {
      top: 130%;
      left: 50%;
    }

    &__item--8 {
      top: 115%;
      left: 70%;
    }
    &__item--9 {
      top: 88%;
      left: 85%;
    }
    &__item--10 {
      top: 60%;
      left: 95%;
    }
    &__item--11 {
      top: 32%;
      left: 85%;
    }
    &__item--12 {
      top: 10%;
      left: 70%;
    }

    &__item-img {
      width: 55px;
    }

    &__main-img {
      position: absolute;
      top: 30%;
      left: 25%;
      max-width: 370px;
      height: 370px;
    }
    &__img-body {
      position: absolute;
      max-width: inherit;
      max-height: inherit;
    }

    &__img-hand1 {
      position: absolute;
      max-width: inherit;
      max-height: inherit;
    }
    &__img-hand2 {
      position: absolute;
      max-width: inherit;
      max-height: inherit;
    }
    &__img-headlight {
      position: absolute;
      max-height: 60px;
      top: 43%;
      left: 95px;
      opacity: 0.5;
    }
    &__img-ellipse {
      position: absolute;
      max-width: inherit;
      max-height: inherit;
      bottom: 0;
    }

  }


</style>
