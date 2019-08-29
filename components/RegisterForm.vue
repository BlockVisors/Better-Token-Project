<template>
  <div id="signup" class="section">
    <div class="container">
      <div class="section-title text-center">
        <h1 id="signup-title">
          Sign Up for <strong>BTRP</strong> Token Airdrop
        </h1>
        <p>Signup with name, email and an Ethereum Address Below</p>
        <p>We will send instructions soon!</p>
      </div>
      <div class="row justify-content-md-center">
        <div class="col col-md-5">
          <form>
            <div class="form-group">
              <input type="text" class="form-control" placeholder="Full Name" />
            </div>
            <div class="form-group">
              <input
                type="email"
                class="form-control"
                placeholder="Email Address"
              />
            </div>
            <div class="form-group">
              <input
                type="password"
                class="form-control"
                placeholder="Password"
              />
            </div>
            <div class="form-group">
              <input
                type="address"
                class="form-control"
                placeholder="ETH Address"
              />
            </div>
            <div class="form-group">
              <button
                id="reg-button"
                type="submit"
                class="btn btn-xl btn-block btn-primary"
              >
                SEND ME FREE BTRP (Better Token Project) Tokens
              </button>
            </div>
          </form>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'RegisterForm'
}
</script>

<style lang="scss">
@import '@/assets/scss/style.scss';
.form-control {
  height: 50px;
  border-radius: 30px;
  padding: 5px 20px;
  height: 55px;
  border-color: #ebebed;
  box-shadow: 0 0 5px rgba(38, 38, 76, 0.05);
}

.btn-block {
  padding: 15px 0;
}
.section-title {
  padding-bottom: 20px;
}
#signup-title {
  font-size: 50px;
  font-weight: 600;
}

// #reg-button {
//   background-color: #35495e;
//   width: 200px;
//   color: #42b883;
//   height: 48px;
// }
</style>
