<template>
  <div id="footer" class="section bg-#42b883 mt-4">
    <div class="container">
      <div class="row">
        <div class="col-sm-3">
          <span class="d-flex flex-row align-items-center">
            <img
              src="https://res.cloudinary.com/codotype/image/upload/v1560045005/tech-logos/codotype.png"
              style="width: 2rem; height: 2rem;"
              class="logo-dark"
              alt="Codotype Logo"
            />
            <p id="logo-txt" class="ml-3 mb-0">
              <span
                >The Better Token Project is a social experiment focused on
                making a better token and making the world a better place.</span
              >
              <br />
            </p>
          </span>
        </div>
        <!-- // end .col-sm-3 -->
        <div class="col-sm-2">
          <ul class="list-unstyled footer-links ml-1">
            <li>
              <nuxt-link to="/generators">
                Story
              </nuxt-link>
            </li>
            <li>
              <a target="_blank" href="https://codotype.org">
                Team
              </a>
            </li>
            <li>
              <nuxt-link to="/generators">
                Tracker
              </nuxt-link>
            </li>
            <li>
              <a target="_blank" href="https://codotype.org">
                Join
              </a>
            </li>
          </ul>
        </div>
        <!-- // end .col-sm-3 -->
        <div class="col-sm-2">
          <ul class="list-unstyled footer-links ml-1">
            <li>
              <nuxt-link to="/about">
                About
              </nuxt-link>
            </li>
            <li>
              <nuxt-link to="/airdrop">
                Airdrop
              </nuxt-link>
            </li>
            <li>
              <nuxt-link to="/faq">
                FAQ
              </nuxt-link>
            </li>
          </ul>
        </div>
        <!-- // end .col-sm-3 -->
        <div class="col-sm-2">
          <ul class="list-unstyled footer-links ml-1">
            <li>
              <a
                target="_blank"
                href="https://github.com/codotype/bettertokenproject"
              >
                GitHub
              </a>
            </li>
            <li>
              <a target="_blank" href="https://twitter.com/bettertokenproject">
                Twitter
              </a>
            </li>
            <li>
              <a
                target="_blank"
                href="https://instagram.com/bettertokenproject"
              >
                Instagram
              </a>
            </li>
            <li>
              <a target="_blank" href="https://twitter.com/codotype">
                Telegram
              </a>
            </li>
            <li>
              <a target="_blank" href="https://twitter.com/codotype">
                Medium
              </a>
            </li>
          </ul>
        </div>
        <!-- // end .col-sm-3 -->
        <div class="col-sm-2">
          <a
            href="#home"
            class="btn btn-sm btn-outline-dark ml-5"
            color="white"
          >
            Go to Top
          </a>
        </div>
        <!-- // end .col-sm-3 -->
      </div>
      <!-- // end .row -->
      <div class="text-center mt-4">
        <small class="text-white">
          Copyright © {{ new Date().getFullYear() }}
          Codotype Inc. All rights reserved.
        </small>
      </div>
    </div>
    <!-- // end .container -->
  </div>
</template>

<script>
export default {
  name: 'Footer'
}
</script>

<style lang="scss">
@import '@/assets/scss/style.scss';

#logo-txt {
  font-size: 12px;
  color: azure;
}
.footer-links {
  li {
    padding: 0.3em 0;
  }
  a {
    color: #35495e;
    &:hover {
      text-decoration: none;
      color: $brand-primary;
    }
  }
}

#footer {
  color: #35495e;
  background-color: #42b883;
  max-height: 380px;
}
.list-unstyled footer-links ml-1 {
  font-weight: bold;
}
.row {
  padding: 22px 22px;
}
</style>
