<script setup>
import { ref } from 'vue';

defineProps({
    msg: String,
})

const count = ref(0)
</script>

<template>
    <form class="login-form mt-5">
        <div class="form-icon primary-bg">
            <span><i class="fa fa-user"></i></span>
        </div>
        <h3 class="mb-5">Login</h3> <!-- Lagay dito yung title ng thesis nila or whatever-->
        <div class="input-group mb-3">
            <span class="input-group-text primary-bg">
                <i class="text-white fa fa-envelope"></i>
            </span>
            <div class="form-floating">
                <input type="email" class="form-control" id="email" placeholder="Email">
                <label for="email">Email</label>
            </div>
        </div>
        <div class="input-group mb-3">
            <span class="input-group-text primary-bg">
                <i class="text-white fa fa-lock"></i>
            </span>
            <div class="form-floating">
                <input type="password" class="form-control" id="password" placeholder="Password">
                <label for="password">Password</label>
            </div>
        </div>
        <div class="d-grid">
            <button class="btn primary-bg" type="submit">Submit</button>
        </div>
    </form>
</template>

<style scoped>
    .primary-bg {
        background-color: #5891ff;
    }
    .login-form{
        background-color: #fff;
        max-width: 600px;
        margin: auto;
        padding: 50px 70px;
        border-radius: 30px;
        box-shadow: 0px 2px 10px rgba(0, 0, 0, 0.075);
    }

    .login-form .form-icon{
        text-align: center;
        border-radius: 50%;
        font-size: 40px;
        color: white;
        width: 100px;
        height: 100px;
        margin: auto;
        margin-bottom: 50px;
        line-height: 100px;
    }

    .login-form button{
        border-radius: 30px;
        padding: 10px 20px;
        font-size: 18px;
        font-weight: bold;
        border: none;
        color: white;
        margin-top: 20px;
    }

    button:hover{
        background-color: #1F69FF;
    }
</style>