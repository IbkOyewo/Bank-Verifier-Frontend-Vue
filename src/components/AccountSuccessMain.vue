<template>
  <main>
      <div class="main-left">
          <h1 class="main-head">Account created<br/>successfully</h1>
          <p class="main-text">{{ text }}</p>

      </div>
      <div class="main-img">

          <img src="../assets/bg-img.png" alt="img" />
      </div>
  </main>
</template>

<script>

export default {
    name: 'AccountSuccessMain',
    data () {
        return {
            text: 'A mail has been sent to verify your account'
        }
    }
}
</script>

<style>
    main {
        display: flex;
        flex-direction: row;
        width: 100%;
        margin-top: 80px;
    }
    .main-left {
        text-align: left;
        padding: 20px;
        margin-left: 140px;
        margin-top: 40px;
        color: #d3484a;
        width: 50%;   
    }
    .main-head {
        font-size: 46px;
    }
    .main-text {
        font-weight: 100;
        width: 60%;
    }
     .cta {
        display: flex;
        flex-direction: row;
        margin-top: 40px;
    }
    .email-input {
        padding: 13px;
        outline: none;
        border: 1px solid #F29091;
        font-family: 'Poppins';
        font-size: 14px;
        border-radius: 8px;
        margin-right: 20px;
    }
    .main-start-btn {
        background-color: #F29091;
        padding: 13px;
        border: none;
        outline: none;
        color: #fff;
        font-family: Poppins;
        font-size: 14px;
        border-radius: 8px;
        font-weight: 400;
        cursor: pointer;
    }
    .main-start-btn:hover {
        background: #c2999a;
    }
    .main-img {
        width: 50%;
    }
</style>