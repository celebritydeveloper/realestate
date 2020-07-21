<template>
    <div>
        <header class="header">
            <slot>
                <Nav />
            </slot>

    </header>

    <main class="body">
        <slot>
        <div class="jumbotron text-center">
        <div class="container">
            <h1 class="display-3 sm-display-5">Buy and Rent Property <br/>any where in Nigeria</h1>
            <p class="lead">Find modern and affordable properties for sale or rent <br /> instantly for your comfort zone.</p>
        </div>
        </div>
        <form class="form-inline justify-content-center align-items-center mx-auto py-3 position-relative search--form">
            <div class="form-group mb-2">
                <input type="text" class="form-control-plaintext search--form-input" id="staticEmail2" placeholder="Enter your location">
            </div>
            <div class="form-group mx-sm-3 mb-2">
                <input type="text" class="form-control-plaintext search--form-input" id="inputPassword2" placeholder="Area or city">
            </div>
            <button type="submit" class="button button-brown btn-lg mb-2 text-white">Search Property</button>
        </form>

        <div class="container steps mb-5">
            <div class="row">
                <div class="col-xm-12 col-sm-12 col-md-5 col-lg-5 col-xl-5">
                    <p class="h1 text-left mb-4">Just follow our steps <br /> and get everything ready</p>
                    <div class="step">
                        <p class="step__timeline">
                            <span class="step--check-mark"><font-awesome-icon icon="check"></font-awesome-icon></span>
                            <span class="step--line"></span>
                        </p>
                        <p class="step--text">
                            <span class="step--title">Find a house you want</span>
                            Visit our website and browse any house of your choice
                        </p>
                    </div>

                    <div class="step">
                        <p class="step__timeline">
                            <span class="check-mark-inactive"><font-awesome-icon icon="check"></font-awesome-icon></span>
                            <span class="step--line step--line-inactive"></span>
                        </p>
                        <p class="step--text">
                            <span class="step--title">Buy your choice</span>
                            Visit our website and browse any house of your choice
                        </p>
                    </div>

                    <div class="step">
                        <p class="step__timeline">
                            <span class="check-mark-inactive"><font-awesome-icon icon="check"></font-awesome-icon></span>
                            <span class="step--line step--line-inactive"></span>
                        </p>
                        <p class="step--text">
                            <span class="step--title">Contact Agent</span>
                            Call agent when ready to inspect or buy or rent property.
                        </p>
                    </div>
                </div>

                <div class="col-md-6 offset-md-1 d-none d-sm-block">
                    <img src="../assets/images/property-4.jpg" class="img-fluid rounded" height="300" alt="">
                </div>  
            </div>
        </div>

        <div class="container">
            <div class="row">
                <div class="col-xm-12 col-sm-12 col-md-5 col-lg-5 col-xl-5">
                    <div class="card">
                        <img src="" alt="">
                        <p class="display-4">520+</p>
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolorum, facere!</p>
                    </div>
                </div>
            </div>
        </div>

        <Property />
        
        </slot>
    </main>
    <footer class="footer">
        <slot>
            <div class="container">
                <div class="row flex flex-row justify-content-center align-items-center">
                    <div class="col-md-3">
                        <p>&copy; Oak Real Estate</p>
                    </div>
                    <div class="col-md-6">
                        <ul class="navbar-nav flex flex-row justify-content-center">
                        <li class="nav-item px-3">
                            <router-link to="/">FAQ </router-link>
                        </li>
                        <li class="nav-item px-3">
                            <router-link to="/">Partners</router-link>
                        </li>
                        <li class="nav-item px-3">
                            <router-link to="/">Contact</router-link>
                        </li>
                        <li class="nav-item px-3">
                            <router-link to="/">Terms and Conditions</router-link>
                        </li>
                        <li class="nav-item px-3">
                            <router-link to="/">Privacy Policy</router-link>
                        </li>
                    </ul>
                    </div>
                    <div class="col-md-3">
                        <router-link to="/" class="px-2">
                            <font-awesome-icon :icon="['fab', 'facebook']" />
                        </router-link>
                        <router-link to="/" class="px-2">
                            <font-awesome-icon :icon="['fab', 'instagram']" />
                        </router-link>
                        <router-link to="/" class="px-2">
                            <font-awesome-icon :icon="['fab', 'twitter']" />
                        </router-link>
                        <router-link to="/" class="px-2">
                            <font-awesome-icon :icon="['fab', 'pinterest']" />
                        </router-link>
                    </div>
                </div>
                
                

            </div>
        </slot>
    </footer>
    </div>
</template>

<script>
import bg from '../assets/images/register-bg.jpg';
import Nav from '../components/Nav';
import Property from '../components/Property';
export default {
    data() {
        return {
            currentRoute: window.location.pathname,
            bg,
        }
    },
    components: {
        Nav,
        Property,
    }
}
</script>

<style lang="scss" scoped>
    // .header {
    //     background: rgb(235,251,254);
    //     height: 450px;
    // }

    .header nav a {
        color: rgb(65, 76, 83);
    }

    .brand-logo img {
        height: auto;
        width: 90px;
    }

    .search--form {
        background: #fff;
        border-radius: 6px;
        box-shadow: 3px 3px 15px rgb(184, 184, 184);
        bottom: 70px;
        width: 50%;
    }

    .search--form-input:focus {
        border: none;
        outline: 0;
    }

    .step {
        display: flex;
        justify-content: space-between;
    }

    .step__timeline {
        align-items: center;
        border: 1px solidred;
        display: flex;
        flex-direction: column;
        justify-content: center;
    }

    .step--check-mark {
        align-items: center;
        background: rgb(189,139,40);
        border-radius: 50%;
        color: #fff;
        display: flex;
        font-size: 1.3rem;
        height: 60px;
        justify-content: center;
        width: 60px;
    }

    .check-mark-inactive{
        align-items: center;
        background: #fff;
        border: 2px solid rgb(189,139,40);
        border-radius: 50%;
        color: rgb(189,139,40);
        display: flex;
        font-size: 1.3rem;
        height: 60px;
        justify-content: center;
        opacity: 0.5;
        width: 60px;
    }

    .step--line {
        background: rgb(189,139,40);
        color: #fff;
        display: flex;
        height: 50px;
        margin-top: 10px;
        width: 5px;
    }

    .step--line-inactive {
        opacity: 0.5;
    }

    .step--text {
        display: flex;
        flex-direction: column;
        font-size: 1.1rem;
    }

    .step--title {
        font-size: 1.3rem;
        font-weight: bold;
        margin-bottom: 10px;
    }


    .footer {

  a {
    font-weight: 500;
    color: #2c3e50;

    &.router-link-exact-active {
      color: rgb(65, 76, 83);
    }
  }
}
</style>
