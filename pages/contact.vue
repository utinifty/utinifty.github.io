<template>
  <main class="contact--us">
    <section class="contact--header">
      <div class="container">
        <div class="header--text">
          <h3>Contact Us</h3>
          <p>
            Let us meet to discuss the future of your projects Send us a message
            right here or contact us through any of the channels listed below
          </p>
        </div>
      </div>
    </section>
    <section class="contact--box">
      <div class="container">
        <div class="contact--heading">
          <h3>Let’s start a conversation</h3>
          <p>
            We believe in a future with abundant opportunities and prosperity
            for all and the role of technology towards achieving this future.
          </p>
        </div>
        <div class="contact--bar-form">
          <div class="contact--bar">
            <div class="">
              <div class="icon-text">
                <img alt="Sms" src="/sms.png" />
                <h4>Email</h4>
              </div>
              <span>ehapamary50@gmail.com</span>
            </div>
            <div class="">
              <div class="icon-text">
                <img alt="Sms" src="/call.png" />
                <h4>Phone Number</h4>
              </div>
              <span>+23407035585261</span>
            </div>
            <div class="">
              <div class="icon-text">
                <img alt="Sms" src="/location.png" />
                <h4>Address</h4>
              </div>
              <span
                >No 10, Plaza B Plateau <br />State, Jos South, Nigeria</span
              >
            </div>
            <div class="">
              <div class="icon-text">
                <img alt="Sms" src="/timer-start.png" />
                <h4>Opening Times</h4>
              </div>
              <span>
                Monday to Fridays <br />
                (8.00AM to 8:00PM)</span
              >
            </div>
          </div>
          <div class="contact--form">
            <h3>Drop Us a Line</h3>
            <form>
              <vs-input label-placeholder="Your Name" />
              <vs-input label-placeholder="Your Email" />
              <vs-textarea label="Message" />
              <div class="">
                <vs-button color="#07b9ed" size="large" type="filled"
                  >Send a message
                </vs-button>
              </div>
            </form>
          </div>
        </div>
      </div>
    </section>
  </main>
</template>

<script>
export default {
  name: 'IndexPage',
}
</script>
<style lang="scss">
.contact--header {
  min-height: 85vh;
  background: url('/contact-us.png') no-repeat;
  background-size: cover;
  padding-top: 100px;
  padding-bottom: 80px;
  display: flex;
  align-items: center;
  justify-content: center;

  .container {
    display: flex;
    align-items: center;
    justify-content: center;

    .header--text {
      max-width: 800px;
      text-align: center;

      h3 {
        font-size: 2.2rem;
        color: #fafafa;
        font-weight: 900;
      }

      p {
        color: #fafafa;
      }
    }
  }
}

.contact--box {
  padding-bottom: 80px;

  .container {
    padding: 40px;
    border-radius: 16px;
    background: #fafafa;
    box-shadow: 0 0 15px -4px;
    margin-top: -50px;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;

    .contact--heading {
      max-width: 750px;
      text-align: center;
      margin-bottom: 50px;

      h3 {
        font-size: 2.2rem;
        font-weight: 600;
      }
    }

    .contact--bar-form {
      display: grid;
      width: 100%;
      grid-template-columns: 40% 60%;

      .contact--bar {
        display: grid;
        grid-gap: 10px;

        .icon-text {
          display: flex;
          align-items: center;
          margin-bottom: 5px;

          img {
            object-fit: contain;
            margin-right: 10px;
            height: 24px;
          }

          h4 {
            font-weight: 600;
          }
        }
      }

      .contact--form {
        background: #ffffff;
        box-shadow: 0px 275px 165px rgba(0, 0, 0, 0.05),
          0px 122px 122px rgba(0, 0, 0, 0.09), 0px 31px 67px rgba(0, 0, 0, 0.1),
          0px 0px 0px rgba(0, 0, 0, 0.1);
        border-radius: 16px;
        padding: 50px;
        display: grid;
        grid-gap: 30px;

        h3 {
          text-align: center;
          font-size: 2rem;
          font-weight: bold;
          color: #07b9ed;
        }

        .vs-con-input-label {
          width: 100%;
          margin-top: 0;
        }

        form {
          display: grid;
          grid-gap: 25px;
        }
      }
    }
  }
}
</style>
