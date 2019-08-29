<template>
  <div id="container">
    <div id="feat-row">
      <b-card>
        <b-media>
          <b-row>
            <b-col md="6">
              <b-img
                slot="aside"
                blank
                blank-color="#ccc"
                width="600"
                height="420"
                alt="placeholder"
              ></b-img>
            </b-col>
            <b-col md="6">
              <h2 class="mt-0">Better Token <strong>(BTRP)</strong> Story</h2>
              <p class="feat-desc">
                The Better Token Project was born from a need to create better
                tokens. We noticed that many tokens created from ICOs(Initial
                Coin Offerings) tend to lose value quickly. These tokens have no
                real long-term viability because they have no basis for value or
                reason for a user to desire to hold them. Some common issues are
                listed below:
              </p>
              <p class="feat3">
                No Element of Scarcity.
              </p>
              <p class="feat3">
                No Value or incentive to re-acquire after using on platform.
              </p>
              <p class="feat3">
                No test or case study for actual "utility"
              </p>
              <p class="feat3">
                No reason to trade or hold- these are essentially the same
                because a trade needs a partner who would like to acquire on the
                other end of the equation.
              </p>
              <p class="feat2">
                Donec sed odio dui. Nullam quis risus eget urna mollis ornare
                vel eu leo. Cum sociis natoque penatibus et magnis dis
                parturient montes, nascetur ridiculus mus.
              </p>
            </b-col>
          </b-row>
        </b-media>
      </b-card>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {}
  },
  methods: {
    onClick() {}
  }
}
</script>

<style scoped>
#container {
  background-color: #42b883;
  color: #35495e;
}

#feat-row {
  margin-top: 60px;
}
.mt-0 {
  padding-top: 30px;
  padding-left: 40px;
  padding-right: 40px;
  padding-bottom: 10px;
  font-size: 40px;
}
.feat-desc {
  padding-top: 20px;
  padding-left: 40px;
  padding-right: 40px;
  padding-bottom: 10px;
  /* margin-left: 30px;
  margin-right: 30px; */
  font-size: 16px;
}
.feat2 {
  padding-top: 20px;
  padding-left: 40px;
  padding-right: 40px;
  padding-bottom: 10px;
  /* margin-left: 30px;
  margin-right: 30px; */
  font-size: 16px;
}

.feat3 {
  padding-top: 5px;
  padding-left: 50px;
  padding-right: 50px;
  padding-bottom: 5px;
  /* margin-left: 30px;
  margin-right: 30px; */
  font-size: 14px;
}
#b-col {
  border-radius: 5px;
}
</style>
