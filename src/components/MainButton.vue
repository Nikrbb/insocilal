<template>
  <button class="main-btn">
    <span class="main-btn__text">{{ message }}</span>
  </button>
  <slot></slot>
</template>

<script>
export default {
  name: 'MainButton',
  data() {
    return {
      message: 'GET STARTED'
    }
  }

}

</script>

<style lang="scss">


.main-btn {
  padding: 16px 34px;
  border: 2px dashed #07166C;
  border-radius: 8px;
  background: #38D89A;

  &__text {
    font-size: 18px;
    line-height: 22px;
    color: #07166C;
    font-weight: bold;
  }

  &:hover {
    border: 2px solid #07166C;
  }
}
</style>