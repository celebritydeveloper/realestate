<template>
  <div class="container register container-sm container-md container-lg container-xl">
      <div class="row">
          <div class="col-sm-12 col-xm-12 col-md-12 col-lg-12 col-xl-12 mb-3 mb-md-5 mb-lg-5 register--logo">
              <router-link to="/" class="px-2"><img :src="logo" alt=""></router-link>
          </div>
      </div>
      <div class="row register--row">
          <div class="col-sm-12 col-xm-12 col-md-5 col-lg-5 col-xl-5 d-none d-sm-block register--bg"></div>
          <div class="col-sm-12 col-xm-12 offset-1 col-md-6 col-lg-6 col-xl-6 register__form">
            <h5 class="h2 mb-2">Create Your Account</h5>

          <form id="register-form">
            <div class="form-row">
              <div class="col-md-10 mb-3">
                <label for="businessName">Full Name</label>
                <input
                  type="text"
                  class="form-control"
                  id="businessName"
                  value=""
                  name="name"
                />
                <div class="valid-feedback d-none" id="valid-feedback-1">
                  Looks good!
                </div>
              </div>
            </div>

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

            <div class="form-row">
              <div class="col-md-10 mb-3 d-none" id="confirm-password">
                <label for="confirmPassword">Confirm Password</label>
                <input
                  type="password"
                  class="form-control"
                  id="confirmPassword"
                  name="cPassword"
                />
                <div class="invalid-feedback d-none" id="invalid-feedback-4">
                  Password must match
                </div>
                <div class="valid-feedback d-none" id="valid-feedback-3">
                  Password matches
                </div>
              </div>
            </div>
            <div class="form-row">
              <div class="col-md-10 mb-3">
                <label for="location">State</label>
                <select class="custom-select" id="location" name="location">
                  <option selected disabled value="">Choose a state...</option>
                </select>
                <div class="invalid-feedback d-none" id="valid-feedback-5">
                  Please select a valid state.
                </div>
              </div>
            </div>
            <small class="text-center">
              By creating an account you agree to RealEstate
              <a href="#">Terms</a> and <a href="#">Conditions</a>.
            </small>
            <br>
            <small class=" text-center">Already have an account? <router-link to="/login/" class="px-2">Login</router-link></small>
            <div class="mt-3 text-center">
              <div class="col-md-10 text-center">
                <button class="button button-brown btn-lg btn-wide text-white" id="sub" type="submit">
                  CREATE ACCOUNT
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
    .register {
        border-radius: 5px;
        margin: 35px auto 0px auto;
    }

    .register--bg {
        background: linear-gradient(to bottom, rgba(84, 99, 110, 0.6), rgba(84, 99, 110, 0.6)), url('../assets/images/property-4.jpg') no-repeat;
        background-size: cover;
        background-position: contain;
        height: 480px;
    }

    .register__form {
        padding: 15px 10px;
    }


    .register--logo {
        display: flex;
        justify-content: center;
        text-align: center;
    }
 

    .register--logo img {
        height: auto;
        width: 120px;
    }
</style>