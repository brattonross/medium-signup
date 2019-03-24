<template>
  <div class="form">
    <h1>Sign In</h1>

    <div class="social-icons">
      <button class="social-button">
        <facebook-icon />
      </button>

      <button class="social-button">
        <google-icon />
      </button>

      <button class="social-button">
        <twitter-icon />
      </button>
    </div>

    <div class="form-splitter">
      <div class="divider" />
      <small class="form-splitter__text">or sign in with email</small>
    </div>

    <div class="form-group">
      <label for="signin-email">Email Address</label>
      <input id="signin-email" type="email" class="form-input">
    </div>

    <div class="form-group">
      <label for="signin-password">Password</label>
      <input id="signin-password" type="password" class="form-input">
    </div>

    <button class="submit-button">Sign In</button>
  </div>
</template>

<script>
import FacebookIcon from 'vue-material-design-icons/Facebook'
import GoogleIcon from 'vue-material-design-icons/Google'
import TwitterIcon from 'vue-material-design-icons/Twitter'

export default {
  components: {
    FacebookIcon,
    GoogleIcon,
    TwitterIcon
  }
}
</script>
