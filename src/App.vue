<template>
  <div id="app">
    <div
      class="container"
      :class="{ 'right-panel-active': showSignUpOverlay }"
    >
      <div class="panel form-container sign-up-container">
        <sign-up-form />
      </div>

      <div class="panel form-container sign-in-container">
        <sign-in-form />
      </div>

      <div class="overlay-container">
        <div class="overlay">
          <div class="panel overlay-panel overlay-left">
            <sign-in-overlay @click="toggleOverlay" />
          </div>

          <div class="panel overlay-panel overlay-right">
            <sign-up-overlay @click="toggleOverlay" />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import SignInForm from './components/SignInForm'
import SignInOverlay from './components/SignInOverlay'
import SignUpForm from './components/SignUpForm'
import SignUpOverlay from './components/SignUpOverlay'

export default {
  name: 'app',
  components: {
    SignInForm,
    SignInOverlay,
    SignUpForm,
    SignUpOverlay
  },
  data: () => ({
    showSignUpOverlay: true
  }),
  methods: {
    toggleOverlay () {
      this.showSignUpOverlay = !this.showSignUpOverlay
    }
  }
}
</script>
