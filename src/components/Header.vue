<template>
  <div class="container">
    <div class="photo">Photo</div>

    <div class="title">WAY KAMBAS <br> MINI EBONY</div>
    <div class="line"></div>

    <div class="description">MATOA Way Kambas Maple comes with a material form of Canadian <br>Maple.</div>

    <div class="discover">Discover</div>

    <div class="actions">
      <div class="calc"> <span class="minus">-</span> 01 <span class="plus">+</span> </div>
      <button class="add"><span class="add__circle"></span>  Add to cart</button>
      <button class="cicil"><img src="../img/image 4.svg" alt=""></button>
    </div>

    <button class="arrow-back"><img src="../img/Vector 1.svg" alt="arrow-back"></button>
    <button class="arrow"><img src="../img/Frame 1.svg" alt="arrow-next"></button>
  </div>
</template>

<script>
export default {
  name: 'TheHeader'
}
</script>

<style scoped lang="scss">
  *{
    font-family: 'Taviraj';
  }
  .container {
    position: relative;
    top: -43px;
    left: 265px;
    width: 1010px;
    height: 505px;
    background: #E5E5E5;
    margin-top: 92px;
    display: flex;
    flex-direction: column;

    .photo {
      position: absolute;
      width: 316px;
      height: 520px;
      left: -98px;
      top: 76px;
      background: #333333;
      display: flex;
      justify-content: center;
      align-items: center;
      text-transform: uppercase;
      font-size: 32px;
      line-height: 55px;
      letter-spacing: 0.02em;
      color: #FFFFFF;
    }

    .title {
      font-size: 60px;
      line-height: 80px;
      letter-spacing: 0.02em;
      color: #333333;
      padding-top: 56px;
      text-align: left;
      margin-left: 280px;
    }

    .line {
      width: 95px;
      height: 2px;
      background: #333333;
      margin-left: 280px;
      margin-bottom: 24px;
    }

    .description {
      font-size: 16px;
      line-height: 27px;
      letter-spacing: 0.02em;
      text-align: left;
      margin-left: 280px;
      margin-bottom: 17px;
      color: #333333;

    }

    .discover {
      font-weight: 600;
      font-size: 16px;
      line-height: 27px;
      letter-spacing: 0.03em;
      margin-left: -386px;
      margin-bottom: 32px;
      color: #333333;
    }
    .discover::before {
      content: '';
      position: absolute;
      top: 336px;
      width: 63px;
      height: 1px;
      background: #333333;
    }

    .actions {
      display: flex;
      justify-content: flex-start;
      align-items: center;
      margin-left: 280px;
      gap: 10px;

      .add {
        width: 229px;
        height: 62px;
        background: #333333;
        font-size: 20px;
        line-height: 34px;
        letter-spacing: 0.02em;
        color: #FFFFFF;
        display: flex;
        justify-content: center;
        align-items: center;
        gap: 17px;
        border: none;
        &__circle {
          display: inline-block;
          width: 28px;
          height: 28px;
          border-radius: 50%;
          background: #C4C4C4;
        }
      }

      .cicil {
        width: 139px;
        height: 62px;
        background: #333333;
        color: #FFFFFF;
        border: none;
      }

      .calc {
        display: flex;
        justify-content: center;
        align-items: center;
        gap: 16px;
        margin-right: 40px;

        .minus {
          width: 24px;
          height: 24px;
          border: 1px solid #ccc;
          color: #ccc;
        }

        .plus {
          width: 24px;
          height: 24px;
          background: #333333;
          color: #fff;
          display: flex;
          justify-content: center;
          align-items: center;
        }
      }
    }

    .arrow {
      position: absolute;
      width: 60px;
      height: 60px;
      left: 919px;
      top: 475px;
      background: #333333;
      color: white;
    }

    .arrow-back {
      position: absolute;
      width: 60px;
      height: 60px;
      left: 840px;
      top: 475px;
      border: 1px solid #333333;
      img {
        transform: rotate(360deg);
      }
    }
  }
</style>
