<template>
  <div id="container">
    <div>
      <b-jumbotron>
        <template slot="header"
          >How It Works</template
        >

        <template slot="lead">
          <div id="token-desc">
            On Every token transfer, 1% of the BTRP Token transaction is burned.
            In addition, we allocate one token to a Cause Wallet that will be
            donated to a selected cause after the end of each month. Tokens are
            all Airdropped, Thus the market will determine the value of the
            token.
          </div>
        </template>

        <hr class="my-4" />

        <p id="tx2">
          1. Signup for the Airdrop
        </p>

        <p class="feat-desc">
          2. Get and Ether Wallet
        </p>
        <p class="feat3">
          3. Recieve Tokens and Send tokens to another Wallet
        </p>
        <p class="feat3">
          4. Share with friends or use mulitple wallets to increase the
          donations and scarcity.
        </p>
        <p class="feat3">
          5. View and Create Causes that can recieve funds.
        </p>
        <p class="feat3">
          6. Check the token tracker as well as analytics on the token to see
          how it is fairing.
        </p>
        <p class="feat2">
          7. Trade for Ether or Bitcoin on exhcanges (Coming soon)
        </p>

        <div id="button-container">
          <b-button id="bb" variant="primary" href="#faq-container" size="lg"
            >FAQ</b-button
          >
          <b-button id="bb" variant="success" href="/Join" size="lg"
            >Join Us</b-button
          >
        </div>
      </b-jumbotron>
    </div>
  </div>
</template>

<script>
// import GeneratorCard from './GeneratorCard.vue'
// import generators from '~/assets/content/generators.json';
import actions from '~/assets/content/actions.json'

export default {
  name: 'BasicJumbo',
  components: {
    // GeneratorCard
  },
  props: {
    title: {
      type: String,
      required: true
    },
    subtitle: {
      type: String,
      required: true
    },
    body: {
      type: String,
      required: true
    }
  },
  data() {
    return {
      actions
    }
  }
}
</script>
<style scoped>
#container {
  padding-top: 110px;
  padding-left: 60px;
  margin-left: 60px;
  margin-right: 60px;
  max-height: 1000px;
}

#tx2 {
  margin-top: 30px;
  margin-bottom: 30px;
}

#button-container {
  margin-top: 30px;
  margin-bottom: 30px;
}
#bb {
  margin: 8px;
  width: 200px;
}
#token-desc {
  margin-top: 30px;
  margin-bottom: 30px;
}
</style>
