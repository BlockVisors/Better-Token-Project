<template>
  <div id="container">
    <div>
      <b-jumbotron text-variant="white">
        <template slot="header"
          >Airdrop Details</template
        >

        <template slot="lead">
          <div id="tx2">
            This is a simple hero unit, a simple jumbotron-style component for
            calling extra attention to featured content or information.
          </div>
        </template>

        <hr class="my-4" color="#42b883" width="85%" />

        <p id="tx3">
          It uses utility classes for typography and spacing to space content
          out within the larger container.
        </p>

        <p id="details">
          There is no Token Sale. We will airdrop
          <strong>444,444 of the total 888,888 BRTP tokens.</strong>
        </p>
        <p id="details">
          Airdrop 1 will be held July 10, 2019. It will consist of a total of
          <strong>222,222 BRTP Tokens</strong>
        </p>
        <p id="details">
          Airdrop 2 will be held August 1, 2019. It will consist of a total of
          <strong>222,222 BRTP Tokens</strong> as well
        </p>

        <p id="details">
          <strong>222,222 BRTP Tokens</strong> will go to the Better Causes
          Fund. Each month, a number of tokens equal to the number of tokens
          Burnt will be sent to the winning cause
        </p>
        <p id="details">
          <strong>111,111 BRTP Tokens</strong> will go to the community and
          Partner Fund and distributed to our partners and community tasks
        </p>
        <p id="details">
          <strong>111,111 BRTP Tokens</strong> will be split amongst the
          Founding team members.
        </p>
        <div id="button-container">
          <b-button id="bb" variant="primary" href="#signup" size="lg"
            >Join Airdrop</b-button
          >
          <b-button id="bb" variant="success" href="/submitCause" size="lg"
            >Create a Cause</b-button
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
  name: 'AirdropJumbo',
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
  padding-bottom: 40px;
  padding-left: 60px;
  max-height: 1200px;
  background-color: #35495e;
  align-content: center;
  text-align: center;
}

#tx2 {
  margin-top: 30px;
  margin-bottom: 30px;
  font-size: 20px;
}
#tx3 {
  margin-top: 30px;
  margin-bottom: 30px;
  padding-bottom: 30px;
  font-size: 20px;
}

#button-container {
  margin-top: 30px;
  margin-bottom: 30px;
  padding-bottom: 30px;
}

#details {
  margin-top: 20px;
  margin-bottom: 20px;
  font-size: 16px;
}
#bb {
  margin: 12px;
}
</style>
