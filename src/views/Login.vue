<template>
  <div class="container login container-sm container-md container-lg container-xl">
      <div class="row">
          <div class="col-sm-12 col-xm-12 col-md-12 col-lg-12 col-xl-12 mb-3 mb-md-5 mb-lg-5 login--logo">
              <router-link to="/" class="px-2"><img :src="logo" alt=""></router-link>
          </div>
      </div>
      <div class="row login--row">
          <div class="col-sm-12 col-xm-12 col-md-5 col-lg-5 col-xl-5 d-none d-sm-block login--bg"></div>
          <div class="col-sm-12 col-xm-12 offset-1 col-md-6 col-lg-6 col-xl-6 login__form">
            <h5 class="h2 mb-5">Login to Your Account</h5>

          <form id="login-form">
            <div class="form-row">
              <div class="col-md-10 mb-3">
                <label for="businessEmail">Email Address</label>
                <input
                  type="text"
                  class="form-control"
                  id="businessEmail"
                  value=""
                  name="email"
                />
                <div class="valid-feedback d-none" id="valid-feedback-1">
                  Looks good!
                </div>
              </div>
            </div>

            <div class="form-row">
              <div class="col-md-10 mb-3">
                <label for="password">Password</label>
                <input type="password" class="form-control" id="password" name="password">
                <span toggle="#password-field" onclick="myFunction()" class="fa fa-fw fa-eye field-icon toggle-password"></span>
                <div class="invalid-feedback d-none" id="invalid-feedback-2">
                  Password is too short.
                </div>
                <div class="valid-feedback d-none" id="valid-feedback-2">
                  Password is secure!
                </div>
              </div>
              <!--<div class="col-md-1 mt-4">
                <input type="text" class="form-control" value="hi">
              <button type="button" onclick="myFunction()" title="Show Password"><span class="fa fa-eye-slash"></span> Hi</button>
              </div>-->
            </div>
            <small class="text-center">Don't have an account? <router-link to="/register/" class="px-2">Register</router-link></small>
            <div class="mt-3 text-center">
              <div class="col-md-10 text-center">
                <button class="button button-brown btn-lg text-white" id="login" type="submit">
                  Login
                </button>
              </div>
              <!--<p class="mt-2">
              Already have an account? <a href="login.html">Login</a>
            </p>-->
            </div>
            
          </form>
          </div>
      </div>
      
  </div>
</template>

<script>
import logo from '../assets/images/oak-express.png';
export default {
    data() {
        return {
           logo,
           firstName: ''
        }
    }
}
</script>
<style scoped>
    .login {
        border-radius: 5px;
        margin: 35px auto 0px auto;
    }

    .login--bg {
        background: linear-gradient(to bottom, rgba(84, 99, 110, 0.6), rgba(84, 99, 110, 0.6)), url('../assets/images/property-4.jpg') no-repeat;
        background-size: cover;
        background-position: contain;
        height: 480px;
    }

    .login__form {
        padding: 15px 10px;
    }


    .login--logo {
        display: flex;
        justify-content: center;
        text-align: center;
    }
 

    .login--logo img {
        height: auto;
        width: 120px;
    }
</style>