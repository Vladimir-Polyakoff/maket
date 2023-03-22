<template>
  <div class="container">
    <div class="title">Sponsor</div>
    <div class="footer">

      <div class="info">
        <div class="logo">Logo</div>
        <div class="address">Address</div>
        <div class="office">Store & Office<br>
          Jl. Setrasari Kulon III, No. 10-12, Kelurahan <br>Sukarasa Kecamatan Sukasari, Kota Bandung,<br> Jawa Barat, Indonesia
        </div>
        <div class="hour">Office Hour</div>
        <div class="week">
          <span>Monday - Sunday</span>
          <span>10.00 - 18.00</span>
          </div>
      </div>

      <div class="contact-container">
          <div class="title-mini">Get in touch</div>
          <div class="contact-row">
            <div>
              <span class="service_title">Customer<br> Service</span>
              <span class="service_title">Phone</span>
              <span class="service_title">Service<br> Center</span>
            </div>
            <div>
              <span class="num">0811-233-8899</span>
              <span class="num">0811-20277564</span>
              <span class="num">0811-233-8899</span>
            </div>
          </div>
          <div class="circle-container">
            <span class="circle"></span>
            <span class="circle"></span>
            <span class="circle"></span>
            <span class="circle"></span>
            <span class="circle"></span>
          </div>
      </div>
      <div class="useful-container">
        <div class="useful">
          <div class="title-mini">Useful Link</div>
          <div class="useful__card" v-for="card in UsefulList" :key="card">
            {{ card }}
          </div>
        </div>

        <div class="useful">
          <div class="title-mini">Useful Link</div>
          <div class="useful__card" v-for="card in UsefulList" :key="card">
            {{ card }}
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'TheSponsor',

  data () {
    return {
      UsefulList: ['Warranty & Complaints', 'Tracking Order', 'How to Adjust', 'How to Care', 'Repair', 'Terms', 'FAQ']
    }
  }
}
</script>
  <style scoped lang="scss">
    * {
      font-family: 'Taviraj';
    }
    .container {
      .title {
        position: relative;
        top: 93px;
        font-weight: 500;
        font-size: 64px;
        line-height: 109px;
        letter-spacing: 0.02em;
        color: #333333;
        text-transform: uppercase;
        width: 1110px;
        height: 194px;
        background: #E5E5E5;
        margin: 23px auto 0;
        display: flex;
        justify-content: center;
        align-items: center;
      }
      .footer {
        width: 1440px;
        height: 568px;
        background: #C4C4C4;

      }
      .info {
        padding-top: 176px;
        display: flex;
        flex-direction: column;
        align-items: flex-start;
        padding-left: 60px;
        width: 364px;
        .logo {
          font-weight: 400;
          font-size: 24px;
          line-height: 41px;
          letter-spacing: 0.02em;
          color: #333333;
          text-transform: uppercase;
          margin-bottom: 16px;
        }
        .address {
          font-weight: 500;
          font-size: 20px;
          line-height: 34px;
          letter-spacing: 0.02em;
          color: #333333;
          margin-bottom: 2px;
        }
        .office {
          text-align: start;
          font-size: 16px;
          line-height: 27px;
          letter-spacing: 0.03em;
          color: #333333;
          margin-bottom: 16px;
        }
        .hour {
          font-weight: 500;
          font-size: 20px;
          line-height: 34px;
          letter-spacing: 0.02em;
          color: #333333;
          margin-bottom: 2px;
        }
        .week span{
          display: block;
          text-align: start;
          font-size: 16px;
          line-height: 27px;
          letter-spacing: 0.02em;
          color: #333333;
        }
      }
      .contact-container {
        display: flex;
        flex-direction:column;
        position: relative;
        top: -307px;
        right: -420px;
        .title-mini {
          font-weight: 600;
          font-size: 24px;
          line-height: 41px;
          letter-spacing: 0.02em;
          color: #333333;
          text-align: start;
          margin-bottom: 16px;
          &::before {
            content: '';
            position: absolute;
            top: 36px;
            width: 60px;
            height: 1px;
            background: #333333;
          }
        }
        .contact-row {
          display: flex;
        }
        .service_title {
          display: flex;
          flex-direction: column;
          font-weight: 500;
          font-size: 20px;
          line-height: 28px;
          letter-spacing: 0.02em;
          color: #333333;
          text-align: start;
          margin-bottom: 8px;
        }
        .num {
          display: flex;
          font-size: 16px;
          line-height: 27px;
          letter-spacing: 0.03em;
          color: #333333;
          margin-bottom: 8px;
          padding: 16px 0 0 34px;
        }
      }
      .circle-container {
        display: flex;
        gap: 16px;
        padding-top: 32px;
      }
      .circle {
        width: 32px;
        height: 32px;
        border-radius: 50%;
        background: #333333;
      }
      .useful-container {
        position: relative;
        top: -592px;
        right: 204px;
        display: flex;
        justify-content: flex-end;
        gap:100px;
        padding-right: 92px;
        .useful {
          display: flex;
          flex-direction: column;
          align-items: flex-start;
          gap:2px;
            .title-mini {
            font-weight: 600;
            font-size: 24px;
            line-height: 41px;
            letter-spacing: 0.02em;
            color: #333333;
            text-align: start;
            margin-bottom: 16px;
            &::before {
              content: '';
              position: absolute;
              top: 36px;
              width: 60px;
              height: 1px;
              background: #333333;
            }
          }
          &__card {
            font-size: 16px;
            line-height: 32px;
            letter-spacing: 0.03em;
            color: #333333;
          }
        }
      }
    }
  </style>
