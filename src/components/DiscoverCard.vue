<template>
  <div class="container">
    <div class="card">
      <div class="card__title">Luxurious <span>Eyewear</span></div>
      <div class="card__description">See the beauty of exotic world with the <br>luxurious glasses</div>
      <div class="card__discover">Discover Now</div>
      <div class="photo left">Photo</div>
    </div>
    <div class="card card-right">
      <div class="card__title">Comfortable <span>Watches</span></div>
      <div class="card__description card__description-right">Feels the balancing function and beauty in <br> our wooden watches</div>
      <div class="card__discover">Discover Now</div>
      <div class="photo right">Photo</div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'DiscoverCard'
}
</script>

<style scoped lang="scss">
  *{
    font-family: 'Taviraj';
  }
  .container {
    margin-top: 210px;
    display: flex;
    justify-content: center;
    gap: 30px;

    .card {
      display: flex;
      flex-direction: column;
      align-items: flex-start;
      padding:32px  0 0 32px;
      width: 520px;
      height: 270px;
      background: #E5E5E5;
      &__title {
        font-size: 28px;
        line-height: 32px;
        letter-spacing: 0.03em;
        color: #333333;
        margin-bottom: 8px;
        span {
        font-weight: 600;
        }
      }
      &__description {
        font-size: 16px;
        line-height: 24px;
        letter-spacing: 0.03em;
        color: #777777;
        text-align: start;
        margin-bottom: 8px;
      }
      &__discover {
        font-weight: 600;
        font-size: 16px;
        line-height: 27px;
        letter-spacing: 0.03em;
        color: #333333;
        &::after {
          content: '';
          display: block;
          width: 90px;
          height: 1px;
          background: #333333;
        }
      }
    }

    .card-right{
      display: flex;
      flex-direction: column;
      align-items: flex-end;
      padding:32px  32px 0 0;
    }
    .card__description-right {
      text-align: end;
    }

    .photo {
      width: 238px;
      height: 114px;
      background: #333333;
      color: #fff;
      font-size: 24px;
      line-height: 41px;
      letter-spacing: 0.02em;
      color: #FFFFFF;
      text-transform: uppercase;
      display: flex;
      justify-content: center;
      align-items: center;
    }
    .left {
      position: relative;
      top: 32px;
      left: 282px;
    }
    .right {
      position: relative;
      top: 32px;
      right: 282px;
    }
  }
</style>
