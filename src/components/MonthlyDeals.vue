<template>
  <div>
    <div class="title"><span></span>Monthly Deals</div>
    <div class="conteiner">
      <div
        v-for="card in cardLIst"
        :key="card.title"
        class="card"
      >
        <div class="card__photo">{{ card.photo }}</div>
        <div class="card__title">{{ card.title }}</div>
        <div class="card__discount">{{ card.discount }}</div>
        <div class="card__old-price">{{ card.oldPrice }}</div>
        <div class="card__price">{{ card.price }}</div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'MonthlyDeals',

  data () {
    return {
      cardLIst: [
        {
          photo: 'Photo',
          title: 'Singo Maple',
          discount: '20% oOff',
          oldPrice: 'Rp 1.500.000',
          price: 'Rp 1.246.000'
        },
        {
          photo: 'Photo',
          title: 'Singo Ebony',
          discount: '20% oOff',
          oldPrice: 'Rp 1.500.000',
          price: 'Rp 1.246.000'
        },
        {
          photo: 'Photo',
          title: 'Rakai Ebony',
          discount: '15% oOff',
          oldPrice: 'Rp 1.250.000',
          price: 'Rp 1.088.000'
        },
        {
          photo: 'Photo',
          title: 'Way Kambas Mini Maple',
          discount: '20% oOff',
          oldPrice: 'Rp 1.500.000',
          price: 'Rp 1.246.000'
        }
      ]
    }
  }
}
</script>

<style scoped lang="scss">
  * {
    font-family: 'Taviraj';
  }
  .title {
    font-weight: 500;
    font-size: 36px;
    line-height: 40px;
    letter-spacing: 0.02em;
    color: #333333;
    margin: 80px 0 120px 160px;
    text-align: start;
    span {
      display: inline-block;
      margin:0 24px 10px 0;
      width: 171px;
      height: 1px;
      background: #333333;
    }
  }
  .conteiner {
    display: flex;
    justify-content: center;
    gap: 30px;
    margin-bottom: 120px;
  }
  .card {
    width: 235px;
    height: 381px;
    background: #E5E5E5;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    padding-left: 24px;
    margin-bottom: 50px;
    &:hover{
      scale: 1.1;
      background: #C4C4C4;
    }
    &__photo {
      position: relative;
      top: -50px;
      width: 207px;
      height: 221px;
      background: #333333;
      color: #fff;
      display: flex;
      justify-content: center;
      align-items: center;
      font-size: 24px;
      line-height: 41px;
      letter-spacing: 0.02em;
      text-transform: uppercase;
    }
    &__title {
      font-weight: 500;
      font-size: 24px;
      line-height: 32px;
      color: #333333;
      margin-bottom: 4px;
      text-align: start;
      margin-top: -20px;
    }
    &__discount {
      font-size: 16px;
      line-height: 24px;
      color: #777777;
      margin-bottom: 18px;
    }
    &__old-price {
      color:#D93F3F;
      margin-bottom: 12px;
      text-decoration: line-through;
    }
    &__price {
      font-size: 24px;
      line-height: 32px;
      color: #333333;
    }
  }
</style>
