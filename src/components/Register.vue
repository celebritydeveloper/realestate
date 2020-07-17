<template>
  <div class="container register container-sm container-md container-lg container-xl">
      <div class="row">
          <div class="col-sm-12 col-xm-12 col-md-12 col-lg-12 col-xl-12 mb-3 mb-md-5 mb-lg-5 register--logo">
              <img :src="logo" alt="">
          </div>
      </div>
      <div class="row register--row">
          <div class="col-sm-12 col-xm-12 col-md-6 col-lg-6 col-xl-6 d-none d-sm-block register--bg"></div>
          <div class="col-sm-12 col-xm-12 col-md-6 col-lg-6 col-xl-6 register__form">
            <form>
                <div class="form-row">
                    <div class="col-md-6 mb-3">
                    <label for="validationServer01">First name</label>
                    <input type="text" class="form-control is-valid" v-model="firstName" id="validationServer01" required>
                    <div class="valid-feedback">
                        Looks good! {{firstName}}
                    </div>
                    </div>
                    <div class="col-md-6 mb-3">
                    <label for="validationServer02">Last name</label>
                    <input type="text" class="form-control is-valid" id="validationServer02"  required>
                    <div class="valid-feedback">
                        Looks good!
                    </div>
                    </div>
                </div>
                <div class="form-row">
                    <div class="col-md-12 mb-3">
                    <label for="validationServer03">Email Address</label>
                    <input type="email" class="form-control is-invalid" id="validationServer03" required>
                    <div class="invalid-feedback">
                        Please provide a valid Email.
                    </div>
                    </div>
                </div>
                <div class="form-row">
                    <div class="col-md-6 mb-3">
                    <label for="validationServer03">Password</label>
                    <input type="email" class="form-control is-invalid" id="validationServer03" required>
                    <div class="invalid-feedback">
                        Password must be greater than 6 characters
                    </div>
                    </div>
                    <div class="col-md-6 mb-3">
                    <label for="validationServer03">Confirm Password</label>
                    <input type="email" class="form-control is-invalid" id="validationServer03" required>
                    <div class="invalid-feedback">
                        Password Doesn't Match.
                    </div>
                    </div>
                </div>
                <div class="form-group">
                    <div class="form-check">
                    <input class="form-check-input is-invalid" type="checkbox" value="" id="invalidCheck3" required>
                    <label class="form-check-label" for="invalidCheck3">
                        Agree to terms and conditions
                    </label>
                    <div class="invalid-feedback">
                        You must agree before submitting.
                    </div>
                    </div>
                </div>
                <button class="btn btn-success btn-lg" type="submit">Create Account</button>
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
        background: linear-gradient(to bottom, rgba(84, 99, 110, 0.6), rgba(84, 99, 110, 0.6)), url('../assets/images/register-bg.jpg') no-repeat;
        background-size: cover;
        background-position: contain;
        height: 450px;
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