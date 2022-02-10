<template>
  <section class="represent">
    <div class="container">
      <div class="subtitle represent__subtitle">
        <h2 class="subtitle__head">Why INSOCIAL?</h2>
        <span class="subtitle__underline"></span>
        <p class="subtitle__text">Our Instagram marketing services are made for growth. <br>
          Must-have for business, influencers, digital marketing specialists </p>
      </div>
      <div class="represent__animation">

        <ul class="represent__list">
          <li class="represent__item"
              :class="{'represent__item--active' : item.isActive}"
              @click="activateItem(item.src)"
              v-for="item in menuItems"
              :key="item.title">
            <div class="represent__item-label">
              <img class="represent__item-img"
                   :src="item.src"
                   alt="label">
            </div>
            <div class="represent__item-text">
              <h4 class="represent__item-title"
              >{{ item.title }}</h4>
              <p class="represent__item-description"
                 :class="{'represent__item-description--active' : item.isActive}"
              >{{ item.description }}
              </p>
            </div>
          </li>
        </ul>
      <MainButton class="represent__main-btn" />
      </div>
    </div>
  </section>

</template>

<script>
import MainButton from "@/components/MainButton";
export default {
  name: "RepresentSection",
  components: {
    MainButton,
  },
  data() {
    return {
      menuItems: [
        {
          title: 'auto promotion',
          description: 'Auto view stories and interact with them',
          src: require("../assets/social-icons/active_auto_promo.png"),
          isActive: false,
        },
        {
          title: 'auto liking',
          description: 'Liking other people\'s posts',
          src: require('../assets/social-icons/active_liking_icon.png'),
          isActive: true,
        },
        {
          title: 'direct messages',
          description: 'Organize your chats and add tags for your customers',
          src: require('../assets/social-icons/active_messages_icon.png'),
          isActive: false,

        },
        {
          title: 'schedule posting',
          description: 'Plan Instagram posts and Stories',
          src: require('../assets/social-icons/active_posting_icon.png'),
          isActive: false,
        },
        {
          title: 'comment tracker',
          description: 'Track your comments and reply faster',
          src: require('../assets/social-icons/active_comment_icon.png'),
          isActive: false,
        },
        {
          title: 'hashtag generator',
          description: 'Generate hashtags for social media automatically',
          src: require('../assets/social-icons/active_hashtag_icon.png'),
          isActive: false,
        },

      ],
    }
  },
  methods: {
    activateItem(q) {
      console.log(q)
    }
  }
}
</script>

<style lang="scss" scoped>
.represent {
  background-image: url("../assets/represent/represent_backgroung.png");
  background-position: center;
  background-repeat: no-repeat;

  &__subtitle {
    max-width: 580px;
  }

  &__animation {
    display: flex;
  }

  &__list {
    margin: 24px 0 0;
    padding-left: 20px;
    max-width: 530px;
    width: 100%;
  }

  &__item {
    display: flex;
    filter: grayscale(100%);
    align-items: center;
    padding: 4px 36px;
    margin-top: 12px;

    background: #F8F8F8;
    box-shadow: 0px 2px 8px rgba(3, 3, 3, 0.15);
    border-radius: 16px;
    transition: 0.1s;
  }
  &__item--active {
    filter: none;
    background: #FFFFFF;
    border-left: 12px solid #38D89A;
    border-bottom-left-radius: 12px;
    border-top-left-radius: 12px;
  }

  &__item-label {
    width: 52px;
    height: 52px;
  }

  &__item-img {
    width: 100%;
    height: 100%;
  }

  &__item-text {
    margin-left: 24px;
    text-align: left;
    color: #07166C;
  }

  &__item-title {
    text-transform: uppercase;
    font-weight: 600;
    font-size: 16px;
    line-height: 20px;
    margin: 0;
  }

  &__item-description {
    font-size: 14px;
    line-height: 150%;
    display: none;
    margin: 0;
  }
  &__item-description--active {
    display: block;
  }

  //&__main-btn {
  //
  //}
}
</style>