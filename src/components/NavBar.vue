<template>
  <div id="navBar">
    <header>
      <div class="logo">
        <img src="@/assets/logo.svg" alt="Gravity"/>
      </div>
      <nav>
        <ul>
          <li class="signIn"><a href="">Sign In</a></li>
          <li><a href="">Why Gravity</a></li>
          <li><a href="">Pricing</a></li>
          <li><a href="">Features</a></li>
        </ul>
        <button class="menu">
          <img src="@/assets/group2582.svg" alt="group 2582">
          <p>Menu</p>
        </button>
      </nav>
    </header>
  </div>
</template>

<script>
export default {
  name: 'NavBar'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  #navBar {
    @media screen and (max-width: 414px) {
      margin-bottom: 47px;
    }
    header {
      display: flex;
      width: 100vw;
      height: 123px;
      flex-flow: nowrap row;
      justify-content: space-between;
      align-items: center;
      box-sizing: border-box;
      padding: 40px 56px;
      @media screen and (max-width: 414px) {
        height: 99px;
        padding: 60px 24px 0 24px;
      }
      .logo {
        img {
          width: 138px;
          height: 43px;
          transform: translateY(6px);
          color: #22322F;
          border: 0;
          @media screen and (max-width: 768px) {
            width: 79px;
            height: 25px;
          }
          @media screen and (max-width: 414px){
            transform: translateY(4px);
          }
        }
      }
      nav {
        display: flex;
        flex-flow: nowrap row;
        ul {
          display: flex;
          width: 413px;
          flex-flow: nowrap row-reverse;
          justify-content: space-between;
          align-items: center;
          @media screen and (max-width: 768px) {
            display: none;
          }
          .signIn {
            font-family: SFProDisplay-Bold;
            color: #71A89E;
          }
          li {
            color: #303031;
            font-size: 20px;
            font-family: SFProDisplay-Medium;
          }
        }
        .menu {
          display: none;
          @media screen and (max-width: 768px) {
            display: flex;
            width: 99px;
            height: 39px;
            flex-flow: nowrap row;
            justify-content: space-between;
            align-items: center;
            box-sizing: border-box;
            padding: 0 22px;
            border: 1px solid #22322F;
            border: {
              right: 2px solid #22322F;
              bottom: 2px solid #22322F;
            }
            border-radius: 8px;
            background-color: #F9F9F9;
            color: #22322F;
            img {
            }
            p {
              font-size: 12px;
              line-height: 19.2px;
              font-family: SFProDisplay-Bold;
            }
          }
        }
      }
    }
  }
</style>
