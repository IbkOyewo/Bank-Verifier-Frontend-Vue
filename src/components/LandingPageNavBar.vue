<template>
    <div class="nav-bar">

        <div class="logo-img-wrapper">
        <router-link :to="{ name: 'Home'}"> 
            <img class="logo-img" src="../assets/verify-now-logo.svg" alt="logo" width="140" />
        </router-link>
        </div>
        <div id="nav">
             <ul>
                <!-- <li class="nav-links"><router-link :to="{name: 'Home'}">Home</router-link> </li> -->
            </ul>
        </div>
        <div class="btn">
            <router-link :to="{ name: 'Login'}">
                <Button buttonText="Login" btnStyle="login" />
            </router-link>
            <router-link :to="{ name: 'Sign Up'}">
                <Button buttonText="Sign Up For Free" :btnStyle="signUp" />
            </router-link>
        </div>
        <router-view />
  </div>
</template>

<script>
import Button from '@/components/Button.vue'

export default {
    name: 'NavBar',
    components: {
        Button
    },
    data () {
        return {
            signUp: 'sign-up-btn'
        }
    },
}
</script>

<style>
    .nav-bar {
        width: 100%;
        display: flex;
        justify-content: space-around;
    }
    .logo-img-wrapper {
        display: flex;
        flex-direction: row;
        padding-top: 30px;
        margin-top: auto;
        margin-bottom: auto;
    }

    img.logo-img{
        width: 237px;
    }

    ul {
        list-style-type: none;
        display: flex;
        flex-direction: row;
        padding-top: 30px;
        text-decoration: none;
    }
    li {
        margin-right: 50px;
        font-weight: 600;
        color: rgb(137, 145, 167);
        cursor: pointer;
    }
    a {
        text-decoration: none;
        color: rgb(137, 145, 167);
    }
    a:hover {
        color: #F29091;
    }
    .router-link-exact-active {
        color: #F29091;
    }
    .btn {
        display: flex;
        flex-direction: row;
        padding: 10px;
        margin-top: auto;
        margin-bottom: auto;
        padding-top: 30px;
    }
    .login {
        padding: 8px;
        background-color: #fff;
        border: 1px solid #F29091;
        border-radius: 6px;
        outline: none;
        margin-right: 30px;
        width: 90px;
        font-family: 'Poppins';
        font-size: 14px;
        cursor: pointer;
        box-shadow: rgba(0, 0, 0, 0.25) 0px 25px 50px -12px;
    }
    .login:hover {
        background-color: #c2999a;
    }
    .sign-up-btn {
        padding: 10px;
        background-color: #F29091;
        border: none;
        border-radius: 6px;
        outline: none;
        font-family: 'Poppins';
        font-size: 14px;
        cursor: pointer;
        box-shadow: rgba(0, 0, 0, 0.25) 0px 25px 50px -12px;
        color: #fff;
    }
    .sign-up-btn:hover {
        background-color: #c2999a;
    }
</style>