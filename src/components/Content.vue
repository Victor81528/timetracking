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
        <div class="CTA">
          <button>Request early access</button>
        </div>
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
    position: relative;
    top: -123px;
    height: 100vh;
    @media screen and (max-width: 414px) {
      height: auto;
      top: 0;
    }
    main {
      display: flex;
      width: 100vw;
      height: 100%;
      flex-flow: nowrap row;
      justify-content: center;
      align-items: center;
      box-sizing: border-box;
      padding: 0 120px;
      @media screen and (max-width: 1200px) {
        padding: 0 40px;
      }
      @media screen and (max-width: 414px) {
        flex-flow: nowrap column-reverse;
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
          margin: 0;
          padding: 0 37px 0 24px;
        }
        .valueProp {
          font-family: SFProDisplay-Regular;
          color: #22322F;
          margin-bottom: 24px;
          h1 {
            font-size: 48px;
            line-height: 72px;
            margin-bottom: 24px;
            @media screen and (max-width: 1024px) {
              font-size: 27px;
              line-height: 43.2px;
            }
            @media screen and (max-width: 414px) {
              margin-bottom: 16px;
            }
          }
          p {
            font-size: 24px;
            line-height: 32px;
            letter-spacing: -2%;
            @media screen and (max-width: 1024px) {
              font-size: 16px;
              line-height: 25.6px;
            }
          }
        }
        .CTA {
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
      }
      .right {
        display: flex;
        height: 100%;
        align-items: center;
        @media screen and (max-width: 414px) {
          margin-bottom: 48px;
          padding: 0 43px 0 24px;
        }
        img {
          // max-height: 100%;
          object-fit: scale-down;
          @media screen and (max-width: 1440px) {
            width: 100%;
          }
          @media screen and (max-width: 1024px) {
            max-width: 308px;
            height: 297px;
          }
        }
      }
    }
  }
</style>
