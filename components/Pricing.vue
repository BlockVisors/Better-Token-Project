<template>
  <div id="pricing" class="section bg-light py-lg">
    <div class="container">
      <div class="section-title text-center mt-0 mb-5">
        <h2>Join The Movement</h2>
        <p>Take Action Below...Our Community Can Use Your Help</p>
      </div>

      <div class="row">
        <div class="col-lg-4">
          <div class="card pricing">
            <div class="card-body">
              <medium class="text-muted">SUBMIT</medium>
              <h5 class="card-title">$9</h5>
              <ul class="card-text list-unstyled">
                <li>3 Projects</li>
                <li class="plan-muted">Team Collaboration</li>
                <li class="plan-muted">Analytics &amp; Reports</li>
                <li>One User</li>
              </ul>
              <a href="#" class="btn btn-xl btn-outline-primary">
                Submit a Cause
              </a>
            </div>
          </div>
        </div>
        <div class="col-lg-4">
          <div class="card pricing">
            <div class="card-body">
              <medium class="text-muted">AIRDROP</medium>
              <h5 class="card-title">$29</h5>
              <ul class="card-text list-unstyled">
                <li>20 Projects</li>
                <li>Team Collaboration</li>
                <li>Analytics &amp; Reports</li>
                <li>10 Active Users</li>
              </ul>
              <a href="/Airdrop" class="btn btn-xl btn-primary">
                Join Airdrop
              </a>
            </div>
          </div>
        </div>
        <div class="col-lg-4">
          <div class="card pricing">
            <div class="card-body">
              <medium class="text-muted">BROWSE</medium>
              <h5 class="card-title">$149</h5>
              <ul class="card-text list-unstyled">
                <li>Unlimited Projects</li>
                <li>Team Collaboration</li>
                <li>Analytics &amp; Reports</li>
                <li>Priority Support</li>
              </ul>
              <a href="/airdrop" class="btn btn-xl btn-outline-primary">
                Browse Causes
              </a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Pricing'
}
</script>

<style lang="scss">
@import '@/assets/scss/style.scss';

.card {
  transition: all 0.3s ease;
  &:hover {
    margin-top: -5px;
    box-shadow: 0 10px 40px rgba($black, 0.05);
  }
}

.pricing {
  text-align: center;
  padding: 20px;
  border: 0;
  border-radius: 15px;
  margin-bottom: 30px;
  small {
    letter-spacing: 2px;
  }
  .card-title {
    font-size: 65px;
    font-family: $heading-font;
    font-weight: 700;
    margin: 10px 0 15px;
  }
  .plan-muted {
    text-decoration: line-through;
    opacity: 0.5;
  }
  ul {
    line-height: 2.5;
    margin: 0 0 20px;
  }
}
</style>
