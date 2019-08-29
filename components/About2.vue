<template>
  <div id="container">
    <div class="row">
      <div class="col-lg-12">
        <div class="row mt-4">
          <div class="col-lg-12 text-center">
            <img
              class="mb-2"
              width="100px"
              height="100px"
              src="https://res.cloudinary.com/codotype/image/upload/v1560045005/tech-logos/codotype.png"
            />
            <h1 class="display-1">Better Token Project</h1>
          </div>
        </div>

        <div class="row">
          <div class="col-lg-12 text-center">
            <p class="lead">
              The Ethos of the Better token project is to incubate real token
              innovation. Token Economics meets Human Behavioral Studies. Our
              project is kicked off and hopefully funded in the future by the
              BTRP token. It is an airdropped token (No ICO) that attempts to
              “share the wealth” and "spread the word". It acts as a store of
              wealth as well as a way to help others by mobilizing funds.
            </p>
            <div id="support-container">
              <p id="support-text">
                On Every Token Transfer...One Token is Burnt and One token is
                sent to the Better Cause Wallet. At the end of the month, the
                tokens are transferred to the wallet of the winning cause.
              </p>
              <p id="support-text">
                The cause with the most social media posts from unique Posters
                is the winner.
              </p>
              <p id="support-text">
                <strong>This does 2 things:</strong>
              </p>
              <p id="support-text">
                1) Spreads the word about the Better Token Project,
              </p>
              <p id="support-text">
                2) Brings awareness to your cause.
              </p>
            </div>
            <h4 id="be-better">
              Lets Be Better!!
            </h4>

            <div id="button-container">
              <b-button id="bb" href="#signup" size="lg">Join Airdrop</b-button>
              <b-button
                id="bb2"
                variant="outline-dark"
                href="/submitCause"
                size="lg"
                >More Info</b-button
              >
            </div>
          </div>

          <!-- <div
            class="col-lg-12 text-center d-flex flex-column align-items-center"
          >
            <gh-btns-star slug="codotype/codotype" show-count />

            <br />

            <p class="lead mb-0 mt-2">
              <span>Built with </span>
              <font-awesome-icon icon="heart" class="text-danger" />
              <span class="px-1">by</span>
              <a href="https://github.com/dgreen899" target="_blank"
                >@dgreen899</a
              >
            </p>

            <gh-btns-follow class="mt-3" user="dgreen899" show-count />
          </div> -->
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  head() {
    return {
      title: 'Codotype - About',
      meta: [
        {
          property: 'twitter:card',
          content: 'summary'
        },
        {
          property: 'twitter:site',
          value: '@codotype'
        },
        {
          property: 'twitter:creator',
          value: '@aeksco'
        },
        {
          hid: 'description',
          name: 'description',
          content:
            'Instantly generate full-stack boilerplate code with custom CRUD.'
        },
        {
          property: 'og:url',
          content: 'https://codotype.io/about'
        },
        {
          property: 'og:type',
          content: 'website'
        },
        {
          property: 'og:title',
          content: 'Codotype - Building Better Boilerplate'
        },
        {
          property: 'og:description',
          content:
            'Instantly generate full-stack boilerplate code with custom CRUD.'
        },
        {
          property: 'og:image',
          content: 'https://avatars2.githubusercontent.com/u/42126198?s=200&v=4'
        }
      ]
    }
  }
}
</script>
<style scoped>
.lead {
  margin-left: 130px;
  margin-right: 130px;
}
#container {
  background-color: #42b883;
  color: #35495e;
  padding-bottom: 40px;
}
#support-container {
  margin-top: 40px;
  margin-bottom: 40px;
}
#support-text {
  margin-left: 140px;
  margin-right: 140px;
}
#be-better {
  font-size: 30px;
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
  background-color: #35495e;
}
#bb2 {
  margin: 12px;
}
</style>
