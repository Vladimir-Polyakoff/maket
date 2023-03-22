<template>
  <div>
    <div class="title"><span></span>Recent News</div>
    <div class="container">
      <div class="card">
        <div class="sub-title">Where To Travel</div>
        <div class="description">Matoa Where To Travel? <br>Yogyakarta</div>
        <button>Discover</button>
      </div>
      <div class="photo">Photo</div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'RecentNews'
}
</script>

<style scoped lang="scss">
  * {
    font-family: 'Taviraj';
  }
  .title {
    position: relative;
    font-weight: 500;
    font-size: 36px;
    line-height: 40px;
    letter-spacing: 0.02em;
    color: #333333;
    margin: 80px 0 120px 160px;
    text-align: start;
    &::after {
      content: '';
      position: absolute;
      right: 0;
      width: 705px;
      height: 479px;
      // background: #E5E5E5;
        background: #C4C4C4;
    }
    span {
      display: inline-block;
      margin:0 24px 10px 0;
      width: 171px;
      height: 1px;
      background: #333333;
    }
  }
  .container {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    margin-left:160px;

    .card {
      display: flex;
      flex-direction: column;
      align-items: center;
    }

    .sub-title {
      font-size: 16px;
      line-height: 40px;
      letter-spacing: 0.02em;
      color: #777777;
      margin-bottom: 8px;
    }
    .description {
      font-size: 28px;
      line-height: 40px;
      text-align: center;
      letter-spacing: 0.02em;
      color: #333333;
      margin-bottom: 60px;
    }
    button {
      width: 160px;
      height: 58px;
      border: 1px solid #333333;
      font-size: 16px;
      line-height: 27px;
      letter-spacing: 0.02em;
      color: #333333;
      background: inherit;
    }
    .photo {
      position: relative;
      top: -315px;
      left: 334px;
      width: 487px;
      height: 484px;
      background: #333333;
      color: white;
      display: flex;
      justify-content: center;
      align-items: center;
      text-transform: uppercase;
      font-size: 48px;
      line-height: 82px;
      letter-spacing: 0.02em;
    }
  }
  </style>
