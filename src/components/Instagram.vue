<template>
  <div class="container">
    <div class="title">Instagram</div>
    <div class="photo-list">
      <div
        v-for="(photo, index) in list"
        :key="index"
        class="photo"
      >
        {{ photo }}
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'TheInstagram',

  data () {
    return {
      list: ['photo', 'photo', 'photo', 'photo', 'photo']
    }
  }
}
</script>

<style scoped lang="scss">
  *{
    font-family: 'Taviraj';
  }
  .container {
    margin-top: -10px;
    .title {
      position: relative;
      top: 40px;
      margin:0 auto;
      width: 540px;
      height: 79px;
      background: #C4C4C4;
      font-weight: 500;
      font-size: 24px;
      line-height: 41px;
      letter-spacing: 0.03em;
      color: #000000;
      text-transform: uppercase;
      display: flex;
      justify-content: center;
      align-items: center;
    }
    .photo-list {
      display: flex;
      margin-left: 165px;
    }
    .photo {
      display: flex;
      justify-content: center;
      align-items: center;
      width: 222px;
      height: 222px;
      background: #333333;
      font-weight: 500;
      font-size: 24px;
      line-height: 40px;
      letter-spacing: 0.02em;
      color: #FFFFFF;
      text-transform: uppercase;
    }
  }
</style>
