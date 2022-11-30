<template>
  <footer class="">
    <div class="container">
      <img src="/icon.png" alt="Footer Logo" class="footer--logo">
      <div class="social--links">
        <div class="socials">
          <a href="" uk-icon="icon: facebook;ratio: 1.5"></a>
          <a href="" uk-icon="icon: twitter;ratio: 1.5"></a>
          <a href="" uk-icon="icon: linkedin;ratio: 1.5"></a>
        </div>
        <div class="links">
          <a href="#">Home</a>
          <a href="#">About</a>
          <a href="#">Contact</a>
        </div>
      </div>
    </div>
    <div class="container">
      <span>© 2022 Utifnity. All Rights Reserved.</span>
    </div>
  </footer>
</template>

<script>
export default {
  name: "MainFooter"
}
</script>

<style lang="scss">
  footer {
    min-height: 30vh;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    position: relative;
    background:  #1D3557;
    &:before {
      content: '';
      background:  url("/footer-bg.svg") no-repeat;
      background-size: cover;
      position: absolute;
      height: 100%;
      width: 100%;
      left: 0;
      top: 0;
      opacity: .2;
    }
    & > * {
      position: relative;
      &.container {
        position: relative;
        display: flex;
        justify-content: center;
        &:first-of-type {
          min-height: calc(30vh - 80px);
        }
        .social--links {
          display: flex;
          flex-direction: column;
          align-items: center;
          justify-content: center;
          .socials {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            grid-gap: 20px;
            a {
              color: #07B9ED;
              font-size: 1.2rem;
            }
          }
          .links {
            margin-top: 30px;
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            grid-gap: 30px;
            a, a:hover {
              color: #fafafa;
              text-decoration: none !important;
            }
          }
        }
        .footer--logo {
          position: absolute;
          left: 0;
          top: 50%;
          transform: translateY(-50%);
          height: 60px;
          width: 60px;
          object-fit: contain;
        }
        &:last-of-type {
          min-height: 80px;
          border-top: solid 1px #fafafa;
          align-items: center;
          span {
            color: #fafafa;
          }
        }
      }
    }
  }
</style>
