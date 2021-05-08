<template>
  <div id="content">
    <main>
      <div class="left">
        <div class="valueProp">
          <h1>Simple time tracking.<br>
              Powerful reporting.
          </h1>
          <p>Turn your team on to productivity with Gravity the time tracker.</p>
        </div>
        <button>Request early access</button>
      </div>
      <div class="right">
        <img src="@/assets/illustration.svg" alt="Illustration">
      </div>
    </main>
  </div>
</template>

<script>
export default {
  name: 'Content'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  #content {
    display: flex;
    position: relative;
    top: -123px;
    min-height: 100%;
    @media screen and (max-height: 811px) {
      height: 811px;
    }
    @media screen and (max-width: 1024px) {
      height: auto;
    }
    main {
      display: flex;
      width: 100vw;
      flex-flow: nowrap row;
      justify-content: center;
      box-sizing: border-box;
      padding: 0 120px;
      @media screen and (max-width: 1024px) {
        flex-flow: nowrap column-reverse;
        margin-top: calc(123px + 99px);
      }
      @media screen and (max-width: 768px) {
        padding: 0 80px;
      }
      @media screen and (max-width: 414px) {
        padding: 0;
      }
      .left {
        display: flex;
        height: 100%;
        flex-flow: nowrap column;
        justify-content: center;
        margin-right: 32px;
        @media screen and (max-width: 414px) {
          justify-content: flex-start;
          padding: 0 37px 0 24px;
          margin: 0;
        }
        .valueProp {
          font-family: SFProDisplay-Regular;
          color: #22322F;
          margin-bottom: 24px;
          h1 {
            font-size: 48px;
            line-height: 72px;
            margin-bottom: 24px;
            @media screen and (max-width: 768px) {
              font-size: 27px;
              line-height: 43.2px;
              margin-bottom: 16px;
            }
          }
          p {
            font-size: 24px;
            line-height: 32px;
            letter-spacing: -2%;
            @media screen and (max-width: 768px) {
              font-size: 16px;
              line-height: 25.6px;
            }
          }
        }
        button {
          width: 222px;
          height: 64px;
          box-sizing: border-box;
          font-size: 18px;
          line-height: 24px;
          margin-bottom: 40px;
          border: 2px solid #000000;
          border-radius: 8px;
          box-shadow: 3px 3px #333333;
          background-color: #71A89E;
          font-family: SFProDisplay-Bold;
          color: #FFFFFF;
          @media screen and (max-width: 1024px) {
            width: 203px;
            height: 44px;
            font-size: 16px;
          }
          @media screen and (max-width: 414px) {
            margin-bottom: 47px;
          }
        }
      }
      .right {
        display: flex;
        height: 100%;
        align-items: center;
        box-sizing: border-box;
        @media screen and (max-width: 1024px) {
          width: 100%;
          margin-bottom: 120px;
        }
        @media screen and (max-width: 414px) {
          margin-bottom: 48px;
          padding: 0 43px 0 24px;
        }
        img {
          object-fit: scale-down;
          @media screen and (max-width: 1440px) {
            max-width: 100%;
            // width: 617px;
          }
        }
      }
    }
  }
</style>
