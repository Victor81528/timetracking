<template>
  <nav>
    <div class="logo-links">
      <div class="logo">
        <img src="@/assets/logo.svg" alt="Gravity"/>
      </div>
      <ul class="links">
        <li class="signIn"><a href="">Sign In</a></li>
        <li><a href="">Why Gravity</a></li>
        <li><a href="">Pricing</a></li>
        <li><a href="">Features</a></li>
      </ul>
    </div>
  </nav>
</template>

<script>
export default {
  name: 'Nav'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  nav {
    display: flex;
    width: 100vw;
    height: 123px;
    box-sizing: border-box;
    padding: 40px 56px;
    .logo-links {
      display: flex;
      position: relative;
      width: 100%;
      height: 43px;
      flex-flow: nowrap row;
      justify-content: space-between;
      box-sizing: border-box;
      padding: 0 64px;
      .logo {
        transform: translateY(6px);
        img {
          width: 138px;
          height: 43px;
          color: #22322F;
          border: 0;
        }
      }
      .links {
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
</style>
