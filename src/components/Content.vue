<template>
  <div id="content">
    <main>
      <div class="left">
        <div class="valueProp">
          <h1>Simple time tracking.<br>
              reporting.
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
    // height: calc(100vh - 123px);
    main {
      display: flex;
      width: 100vw;
      flex-flow: nowrap row;
      justify-content: center;
      align-items: center;
      box-sizing: border-box;
      padding: 0 120px;
      .left {
        display: flex;
        max-width: 551px;
        flex-flow: nowrap column;
        margin-right: 32px;
        .valueProp {
          font-family: SFProDisplay-Regular;
          color: #22322F;
          margin-bottom: 24px;
          h1 {
            font-size: 48px;
            line-height: 72px;
            margin-bottom: 24px;
          }
          p {
            font-size: 24px;
            line-height: 32px;
            letter-spacing: -2%;
          }
        }
        .CTA {
          button {
            width: 222px;
            height: 64px;
            box-sizing: border-box;
            font-size: 18px;
            line-height: 24px;
            border-radius: 8px;
            border: 2px solid #000000;
            box-shadow: 3px 3px #333333;
            background-color: #71A89E;
            font-family: SFProDisplay-Bold;
            color: #FFFFFF;
          }
        }
      }
      .right {
        img {
          min-width: 617px;
        }
      }
    }
  }
</style>
