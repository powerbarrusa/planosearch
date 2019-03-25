<template>
  <view class="container">
    <text class="logo">PlanOsearch</text>
    <text class="mantra">For every home search</text>
    <text-input
      class="login"
      placeholder="Username"
      v-model="username"
    />
    <text-input
      class="login"
      placeholder="Password"
      v-model="password"
    />
    <touchable-opacity
      :on-press="login"
      class="login_button"
    >
      <text>Login</text>
    </touchable-opacity>
  </view>
</template>

<script>
export default {
  data() {
    return {
      username: "",
      password: ""
    }
  },
  methods: {
    login() {
      alert("Clicked")
    }
  }
}
</script>
 
<style>
.container {
  background-color: white;
  align-items: center;
  justify-content: center;
  flex: 1;
}

.logo {
  color: orangered;
  font-size: 50;
  margin-bottom: 100;
  /* font-family: "Times"; */
}

.mantra {
  color: grey;
  font-size: 15;
  margin-top: -100;
  margin-bottom: 100;
}

.login {
  height: 30;
  width: 300;
  border-color: gray;
  border-width: 2;
  margin: 20;
  margin-bottom: 50;
  border-radius: 5;
}

.login_button {
  background-color: orangered;
  padding: 10;
  border-radius: 5;
}
</style>
