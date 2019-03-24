<template>
  <div class="overlay-content">
    <h1>Welcome back.</h1>
    <p>Sign in to get your personalized statistics, recommendations, and more.</p>
    <button
      class="app-button"
      @click="$emit('click', $event)"
    >
    Sign In
  </button>
  </div>
</template>

<style>
h1 {
  margin: 0;
  font-size: 2.5em;
}
p {
  margin: 3rem 0;
}
</style>
