<script>
export default {
  name: 'TheTestimonials'
}
</script>

<template>
  <div class="container">
      <div class="photo">Photo</div>
      <div class="card">
        <div class="title"><span></span>Testimonials</div>
        <div class="description">Loving my new KAILI watch from @matoa_id, the first ever <br>Indonesian watch local brand that uses wood as their main<br> material. Like any other Matoa products, KAILI is inspired by <br>Indonesian heritage.</div>
        <div class="name">Gita Savitri</div>
        <div class="comment">Content Creator/Influencer</div>
      </div>
      <span class="square"><span></span></span>
      <span class="square-r"><span></span></span>
  </div>
</template>

<style scoped lang="scss">
  * {
    font-family: 'Taviraj';
  }
  .container {
    position: relative;
    width: 520px;
    display: flex;
    flex-direction: column;
    align-items: flex-end;
    text-align:start;
    margin-left:auto;
    padding-right: 250px;
    .photo {
      position: absolute;
      width: 511px;
      height: 321px;
      top: 229px;
      left: -505px;
      background: #333333;
      font-weight: 500;
      font-size: 36px;
      line-height: 40px;
      letter-spacing: 0.02em;
      color: #FFFFFF;
      text-transform: uppercase;
      display: flex;
      justify-content: center;
      align-items: center;
      z-index: 1111;
    }
    .card {
      display: flex;
      flex-direction: column;
    }
    .title {
      position: relative;
      font-weight: 500;
      font-size: 36px;
      line-height: 40px;
      letter-spacing: 0.02em;
      color: #333333;
      margin: 160px 0 80px 0px;
      text-align: end;
      &::after {
        content: '';
        position: absolute;
        width: 515px;
        height: 300px;
        right: 675px;
        top: 0px;
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
    .description {
        font-weight: 300;
        font-size: 16px;
        line-height: 32px;
        letter-spacing: 0.03em;
        color: #333333;
        margin-bottom: 32px;
      }
      .name {
        font-weight: 500;
        font-size: 24px;
        line-height: 32px;
        letter-spacing: 0.03em;
        color: #333333;
      }
      .comment {
        font-weight: 300;
        font-size: 16px;
        line-height: 32px;
        letter-spacing: 0.03em;
        color: #777777;
        margin-bottom: 190px;
      }
      .square {
        position: absolute;
        bottom: 68px;
        left: -504px;
        width: 64px;
        height: 64px;
        background: #E5E5E5;
        display: flex;
        justify-content: center;
        align-items: center;
        span {
          display: block;
          width: 32px;
          height: 32px;
          border-radius: 50%;
          background: #333333;
        }
      }
      .square-r {
        position: absolute;
        bottom: 68px;
        left: -424px;
        width: 64px;
        height: 64px;
        background: #C4C4C4;
        display: flex;
        justify-content: center;
        align-items: center;
        span {
          display: block;
          width: 32px;
          height: 32px;
          border-radius: 50%;
          background: #333333;
        }
      }
  }
</style>
