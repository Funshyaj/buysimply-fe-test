<script setup lang="ts">
import { ref } from 'vue'

const email = ref('')
const password = ref('')
</script>

<template>
  <main>
    <!-- pc side display -->
    <div class="pc-side">
      <div>Team Acheive</div>
    </div>

    <form action="">
      <div>
        <h1>Welcome Back</h1>
        <p>Enter your email address and password to access your account</p>
      </div>
      <div>
        <label for="email">Email Address</label>
        <input
          type="email"
          name="email"
          id="email"
          placeholder="Enter your email"
          required
          v-model="email"
        />
      </div>

      <div>
        <label for="password">Password</label>
        <input
          type="password"
          name="password"
          id="password"
          placeholder="Enter your password"
          required
          v-model="password"
        />
      </div>

      <div>
        <div><input type="checkbox" name="" id="  " /><span>Remember me</span></div>

        <p>Forgot Password</p>
      </div>

      <button type="submit">Sign In</button>
    </form>
  </main>
</template>

<style scoped>
main {
  display: flex;
}

.pc-side {
  background: pink;
}
</style>
