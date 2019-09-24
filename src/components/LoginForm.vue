<template>
<div class="h-screen container mx-auto">
  <div class="h-full flex justify-center items-center">
    <div class="w-full min-w-0 max-w-md ">

      <!-- TITLE SECTION -->
    <div class="z-30 px-20 relative"><div class="pt-5 login__title-top-shadow "></div></div>
    <div class="z-20 -mb-24 px-20 relative"><h1 class="p-5 text-white text-center login__title text-4xl font-bold orange">LOGIN</h1></div>
    <form class="z-0 mt-12 login__form-wrapper rounded-lg px-20 pt-24 pb-12 mb-12">

      <!-- USERNAME FIELD -->
      <div class="mb-6 h-12 rounded login__field flex items-center">
        <div class="w-2/12 py-2 "><img  class="login__user-image relative" src="../assets/images/user.svg" alt=""></div>
        <div class="w-1/12 login__vl py-2 px-0"></div>
        <input class="w-8/12 py-2 rounded bg-transparent appearance-none outline-none text-lg overflow-hidden" id="username" v-model="username" type="text" placeholder="username">
        <!-- <div class="w-1/12 pr-1 py-2"><img  class="login__wrong-image" src="../assets/images/wrong2.svg" alt=""></div> -->
      </div>

      <!-- PASSWORD FIELD -->
      <div class="mb-4 h-12 rounded login__field flex items-center">
        <div class="w-2/12 py-2"><img  class="login__pass-image relative" src="../assets/images/lock.svg" alt=""></div>
        <div class="w-1/12 login__vl py-2 px-0"></div>
        <input class=" w-8/12 py-2 rounded bg-transparent appearance-none outline-none text-lg overflow-hidden" id="password" v-model="password" type="password" placeholder=" ***********">
        <!-- <div class="w-1/12 pr-1 py-2"><img  class="login__wrong-image" src="../assets/images/wrong2.svg" alt=""></div> -->
      </div>

      <!-- FORGET PASSWORD LINK -->
      <div class="w-full mb-10 text-right">
       <a class="text-sm font-medium text-white" href="#">
          Forgot Password?
        </a>
      </div>

      <!-- ERROR MESSAGE -->
      <!-- <div class="w-full -mt-2 mb-10 text-left flex justify-center items-center">
        <img  class="flex-1 login__wrong-image inline pr-1" src="../assets/images/wrong.svg" alt="">
        <p class="flex-1 text-base text-white font-bold inline pl-1">Invaild username or password</p>
      </div> -->

      <!-- SUBMIT BUTTON -->
      <div class="w-full flex ">
        <button class="flex-1 login__submit text-2xl orange rounded p-4 text-white font-bold" type="button">
          SUBMIT
        </button>
      </div>

    </form>
      <!-- COMPONENT SHADOW -->
    <div class="w-full login__shadow"></div>
    </div>
  </div>
</div>
</template>

<script>
export default {
  name: "LoginForm",
  data: function () {
    return {
      username: "",
      password: "",
    };
  },
  method:{
    isEmpty(){

    },

  }
};
</script>
