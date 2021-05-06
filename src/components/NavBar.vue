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
    header {
      display: flex;
      width: 100vw;
      height: 123px;
      flex-flow: nowrap row;
      justify-content: space-between;
      align-items: center;
      box-sizing: border-box;
      padding: 40px 56px;
      .logo {
        img {
          width: 138px;
          height: 43px;
          transform: translateY(6px);
          color: #22322F;
          border: 0;
        }
      }
      nav {
        ul {
          display: flex;
          width: 413px;
          flex-flow: nowrap row-reverse;
          justify-content: space-between;
          align-items: center;
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
      }
    }
  }
</style>
