<template>
  <div>
    <div class="box">
      <div class="title-list">
        <div
          v-for="title in titleList"
          :key="title"
          >
          <div class="title">{{ title }}</div>
        </div>
      </div>
    </div>

    <div class="card-list">
      <div
        v-for="card in cardList"
        :key="card.id"
        class="card"
      >
      <div>
          <div class="card__photo">{{ card.photo }}</div>
      </div>
      <div class="content">
          <div class="card__title">{{ card.title }}</div>
          <div class="card__price">{{ card.price }}</div>
      </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'TheBestseller',
  data () {
    return {
      titleList: ['Bestseller', 'New Arrival', 'Featured'],
      cardList: [
        {
          id: 1,
          title: 'Tomia Maple',
          price: 'Rp 1.280.000',
          photo: 'photo'
        },
        {
          id: 2,
          title: 'Rakai Maple',
          price: 'Rp 1.280.000',
          photo: 'photo'
        },
        {
          id: 3,
          title: 'Tomia Maple',
          price: 'Rp 1.280.000',
          photo: 'photo'
        },
        {
          id: 4,
          title: 'Way Kambas Maple',
          price: 'Rp 1.280.000',
          photo: 'photo'
        },
        {
          id: 5,
          title: 'Alor',
          price: 'Rp 1.170.000',
          photo: 'photo'
        },
        {
          id: 6,
          title: 'Way Kambas Maple',
          price: 'Rp 1.280.000',
          photo: 'photo'
        },
        {
          id: 7,
          title: 'Sunda',
          price: 'Rp 1.170.000',
          photo: 'photo'
        },
        {
          id: 8,
          title: 'Sunda',
          price: 'Rp 1.170.000',
          photo: 'photo'
        },
        {
          id: 9,
          title: 'Sunda',
          price: 'Rp 1.170.000',
          photo: 'photo'
        }
      ]
    }
  }
}
</script>

<style scoped lang="scss">
  .box {
    margin-top: -150px;
  }
  .title-list {
    display: flex;
    justify-content: center;
    margin:0 0 60px -62px;
  }
  .title {
    font-size: 36px;
    line-height: 40px;
    letter-spacing: 0.02em;
    color: #333333;
    margin-right: 26px;
    padding-right: 64px;
    &::before {
      content: "";
      display: inline-block;
      width: 65px;
      height: 1px;
      background: #333333;
      margin-right: 24px;
    }
  }
  .card-list {
    display: flex;
    flex-wrap: wrap;
    gap: 24px;
    margin-left: 165px;
    .card {
      display: flex;
      width: 330px;
      &__photo {
        width: 131px;
        height: 131px;
        background: #333333;
        font-size: 24px;
        line-height: 41px;
        letter-spacing: 0.02em;
        color: #FFFFFF;
        display: flex;
        align-items: center;
        justify-content: center;
        text-transform: uppercase;
      }
      &__title {
        font-size: 24px;
        line-height: 40px;
        letter-spacing: 0.02em;
        color: #333333;
        text-align: start;
      }
      &__price {
        font-size: 28px;
        line-height: 40px;
        letter-spacing: 0.02em;
        color: #333333;
      }
      .content {
        margin-left: 24px;
      }
    }
  }
</style>
