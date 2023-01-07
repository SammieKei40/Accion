<template>
  <div class="container1 pt-5 lg:pt-20 overflow-x-hidden">
    <Nav />
    <div
      class="flex flex-col h-screen place-items-center items-center justify-center"
    >
      <Title class="w-[1256px] h-[110px] hidden md:flex" />
      <div
        class="flex mb-6 mt-auto items-center cursor-pointer rounded-lg m-8 p-3 text-center bg-white text-gray-400"
      >
        <p class="">Quick Banking</p>
        <Green class="items-center" />
      </div>

      <div class="hidden md:flex pb-3 flex-col lg:flex-row gap-5 mb-3">
        <div class="frame">
          <div class="">
            <Account class="text-center" />
            <h1
              class="open-account text-left text-black text-3xl font-bold mt-5"
            >
              Open Account
            </h1>
            <p class="text-gray-300 text-left pt-10 text-2xl">
              New to Accion MFB? Click here to open an account with us.
            </p>
          </div>
        </div>
        <div class="frame">
          <div>
            <Register />
            <h1
              class="open-account text-black text-left text-3xl font-bold mt-5"
            >
              Register
            </h1>
            <p class="text-gray-300 text-left pt-10 text-2xl">
              Already have an offline account with Accion MFB? Click here to
              register.
            </p>
          </div>
        </div>
        <div class="frame">
          <div>
            <Login />
            <h1
              class="open-account text-black text-left text-3xl font-bold mt-5"
            >
              Login
            </h1>
            <p class="text-gray-300 text-left pt-10 text-2xl">
              Already have an offline account with Accion MFB? Click here to
              login
            </p>
          </div>
        </div>
      </div>

      <div class="mt-auto mb-20">
        <div class="flex btn rounded-lg mb-5 cursor-ponter">
          <Google />
          <a href="" class="pl-2 text-white text-xl">Google Play</a>
        </div>

        <div class="flex btn rounded-lg cursor-pointer">
          <Apple />
          <a href="" class="pl-2 text-white text-xl">Apple Store</a>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import Title from "../components/svgs/Title.vue";
import Account from "../components/svgs/Account.vue";
import Register from "../components/svgs/Register.vue";
import Login from "../components/svgs/Login.vue";
import Google from "../components/svgs/Google.vue";
import Apple from "../components/svgs/Apple.vue";
import Green from "../components/svgs/Green.vue";
import Nav from "../components/NavBar/Nav.vue";
</script>

<style scoped>
/* .title {
  font-weight: 900;
  letter-spacing: 0;
  line-height: 40px;
  white-space: nowrap;
}
img {
  height: 24px;
  width: 48px;
} */
.frame {
  align-items: flex-start;
  background-color: white;
  border: 0.5px solid;
  border-color: rgba(0, 0, 0, 0.051);
  border-radius: 10px;
  box-shadow: -10px 10px 25px 5px #e877241a;
  height: 397px;
  overflow: hidden;
  padding: 16px;
  position: relative;
  width: 297px;
}

.open-account {
  letter-spacing: 0.3px;
  line-height: 27px;
  min-width: 118px;
  white-space: nowrap;
}

.btn {
  align-items: center;
  border: 3px solid;
  border-color: rgba(232, 119, 36, 1);
  padding: 0 208px;
  height: 56px;
  /* min-width: 536px; */
}
.container1 {
  width: 100%;
  height: 100vh;
  /* padding-top: 5rem; */
  background: url("../assets/images/Building.jpg");
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center;
  display: flex;
  flex-direction: column;
  align-items: center;
}

@media only screen and (max-width: 600px) {
  .btn {
    padding: 0 90px;
  }
}
</style>
