<template>
  <div class="menu">
    <div class="logo">
      <div class="menu__circle"></div>
      <div class="menu__logo">LOGO</div>
    </div>
    <div class="actions">
      <div v-for="item in list" :key="item" @click="$router.push({name: item === 'practics' ? item : 'home'})">{{ item }}</div>
    </div>
    <div>
      <div class="log-in">
        Log in
        </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'TheMenu',

  data () {
    return {
      list: ['Watches', 'Eyewear', 'Accessories', 'News', 'practics']
    }
  }
}
</script>

<style scoped lang="scss">
  *{
    font-family: 'Taviraj';
  }
  .menu {
    display: flex;
    justify-content: space-between;
    .logo {
      display: flex;
      align-items: center;
      gap: 42px;
      padding: 27px 24px;
    }
    &__circle {
      width: 46px;
      height: 46px;
      background: #000;
      border-radius: 50%;
    }
    &__logo {
      font-size: 40px;
      line-height: 68px;
      letter-spacing: 0.02em;
    }

    .actions {
      display: flex;
      gap: 36px;
      padding-top: 35px;
      font-size: 20px;
      line-height: 34px;
      letter-spacing: 0.02em;
    }

    .log-in {
      padding: 35px 110px 0 0;
      font-size: 18px;
      line-height: 31px;
      letter-spacing: 0.02em;
    }

    .log-in::before {
      content: '';
      position: absolute;
      display: inline-block;
      width: 32px;
      height: 32px;
      border-radius: 50%;
      background: #333333;
      margin-inline: -40px
    }
    .log-in::after {
      content: '';
      position: absolute;
      width: 46px;
      height: 46px;
      background: #000;
      border-radius: 50%;
      margin-left: 40px;
    }
  }
</style>
