<template>
    <div>
        <header class="header">
            <slot>
                <nav class="navbar navbar-expand-lg py-3">
                    <a class="navbar-brand brand-logo" href="/"><img src="../assets/images/oak-express.png" alt=""></a>
                    <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
                        <span class="navbar-toggler-icon"></span>
                    </button>

                    <div class="collapse navbar-collapse" id="navbarSupportedContent">
                        <ul class="navbar-nav mr-auto">
                        <li class="nav-item active">
                            <a class="nav-link" href="#">Home <span class="sr-only">(current)</span></a>
                        </li>
                        <li class="nav-item dropdown">
                            <a class="nav-link dropdown-toggle" href="#" id="navbarDropdown" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                            Buy
                            </a>
                            <div class="dropdown-menu" aria-labelledby="navbarDropdown">
                            <a class="dropdown-item" href="#">Property</a>
                            <a class="dropdown-item" href="#">Land</a>
                            <div class="dropdown-divider"></div>
                            <a class="dropdown-item" href="#">Something else here</a>
                            </div>
                        </li>
                        <li class="nav-item dropdown">
                            <a class="nav-link dropdown-toggle" href="#" id="navbarDropdown" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                            Rent
                            </a>
                            <div class="dropdown-menu" aria-labelledby="navbarDropdown">
                            <a class="dropdown-item" href="#">Property</a>
                            <a class="dropdown-item" href="#">Land</a>
                            <div class="dropdown-divider"></div>
                            <a class="dropdown-item" href="#">Something else here</a>
                            </div>
                        </li>
                        </ul>
                        <div class="inline justify-content-center">
                            <ul class="navbar-nav mr-auto">
                                <li class="nav-item active">
                                    <a class="nav-link" href="/register/">Sign in<span class="sr-only">(current)</span></a>
                                </li>
                                <li class="nav-item active">
                                    <a class="nav-link btn btn-success btn-lg text-white" href="#">Create Account <span class="sr-only">(current)</span></a>
                                </li>
                            </ul>
                        </div>
                    </div>
                </nav>
            </slot>

    </header>

    <main>
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
            <button type="submit" class="btn btn-primary btn-lg mb-2">Search Property</button>
        </form>

        <div class="container steps">
            <div class="row">
                <div class="col-xm-12 col-sm-12 col-md-6 col-lg-6 col-xl-6">
                    <p class="display-4">Just follow our steps <br /> and get everything ready</p>
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

                <div class="col-md-6 d-none d-sm-block">
                    <img :src="property1" class="img-fluid rounded" height="300" alt="">
                </div>  
            </div>
        </div>

        <section class="container-fluid py-5">
            <div class="row">
                <div class="col-xm-6 col-sm-6 col-md-3 col-lg-12 col-xl-3">
                    <div class="card property--card rounded">
                        <img :src="property2" class="card-img-top rounded property-img" height="380" alt="...">
                        <div class="card-footer mx-auto rounded property--footer position-relative">
                            <p class="property--location">Ikeja, Lagos</p>
                            <p class="h5 property--type">2 Bedroom Apartment</p>
                            <div class="property--amenity">
                                <span>
                                    <font-awesome-icon icon="user-secret"></font-awesome-icon>
                                    5 Bed</span>
                                <span>
                                    <font-awesome-icon icon="user-secret"></font-awesome-icon>
                                    3 Bath</span>
                                <span>
                                    <font-awesome-icon icon="user-secret"></font-awesome-icon>
                                    Parking</span>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="col-xm-6 col-sm-6 col-md-3 col-lg-3 col-xl-3">
                    <div class="card property--card rounded">
                        <img :src="property1" class="card-img-top rounded property-img" height="380" alt="...">
                        <div class="card-footer mx-auto rounded property--footer position-relative">
                            <p class="property--location">Ikeja, Lagos</p>
                            <p class="h5 property--type">2 Bedroom Apartment</p>
                            <div class="property--amenity">
                                <span>
                                    <font-awesome-icon icon="couch"></font-awesome-icon>
                                    5 Bed</span>
                                <span>
                                    <font-awesome-icon icon="bath"></font-awesome-icon>
                                    3 Bath</span>
                                <span>
                                    <font-awesome-icon icon="car"></font-awesome-icon>
                                    Parking</span>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="col-xm-6 col-sm-6 col-md-3 col-lg-3 col-xl-3">
                    <div class="card property--card rounded">
                        <img :src="bg" class="card-img-top rounded property-img" height="380" alt="...">
                        <div class="card-footer mx-auto rounded property--footer position-relative">
                            <p class="property--location">Ikeja, Lagos</p>
                            <p class="h5 property--type">2 Bedroom Apartment</p>
                            <div class="property--amenity">
                                <span>
                                    <font-awesome-icon icon="couch"></font-awesome-icon>
                                    5 Bed</span>
                                <span>
                                    <font-awesome-icon icon="bath"></font-awesome-icon>
                                    3 Bath</span>
                                <span>
                                    <font-awesome-icon icon="car"></font-awesome-icon>
                                    Parking</span>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="col-xm-6 col-sm-6 col-md-3 col-lg-3 col-xl-3">
                    <div class="card property--card rounded">
                        <img :src="property3" class="card-img-top rounded property-img" height="380" alt="...">
                        <div class="card-footer mx-auto rounded property--footer position-relative">
                            <p class="property--location">Ikeja, Lagos</p>
                            <p class="h5 property--type">2 Bedroom Apartment</p>
                            <div class="property--amenity">
                                <span>
                                    <font-awesome-icon icon="couch"></font-awesome-icon>
                                    5 Bed</span>
                                <span>
                                    <font-awesome-icon icon="bath"></font-awesome-icon>
                                    3 Bath</span>
                                <span>
                                    <font-awesome-icon icon="car"></font-awesome-icon>
                                    Parking</span>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
             
        </section>

              
        
        </slot>
    </main>
    <footer>
        <slot>
            <div class="container">
                <div class="row">
                    <div class="col-md-3">
                        <p>&copy; Oak Real Estate</p>
                    </div>
                    <div class="col-md-6">
                        <p>&copy; Oak Real Estate</p>
                    </div>
                    <div class="col-md-3">
                        <a href="#">
                            <font-awesome-icon icon="bath"></font-awesome-icon>
                        </a>
                        <a href="#">
                            <font-awesome-icon icon="car"></font-awesome-icon>
                        </a>
                        <a href="#">
                            <font-awesome-icon icon="car"></font-awesome-icon>
                        </a>
                    </div>
                </div>
                
                

            </div>
        </slot>
    </footer>
    </div>
</template>

<script>
import bg from '../assets/images/register-bg.jpg';
import property1 from '../assets/images/property-1.jpg';
import property2 from '../assets/images/property-2.jpg';
import property3 from '../assets/images/property-3.jpg';
const Home = { template: '<p>home page</p>' }
const About = { template: '<p>about page</p>' }
export default {
    data() {
        return {
            currentRoute: window.location.pathname,
            bg,
            property1,
            property2,
            property3,
        }
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
        background: red;
        border-radius: 50%;
        color: #fff;
        display: flex;
        font-size: 1.5rem;
        height: 60px;
        justify-content: center;
        width: 60px;
    }

    .check-mark-inactive{
        align-items: center;
        background: #fff;
        border: 2px solid red;
        border-radius: 50%;
        color: red;
        display: flex;
        font-size: 1.5rem;
        height: 60px;
        justify-content: center;
        opacity: 0.5;
        width: 60px;
    }

    .step--line {
        background: red;
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

    .property--card {
        border: none;
    }

    .property-img {
        object-fit: cover;
    }

    .property--footer {
        background: #fff;
        border: none;
        border-radius: 10px;
        bottom: 50px;
        box-shadow: 1px 3px 10px rgb(201, 195, 195);
        padding: 20px 15px;
        width: 90%;
    }

    .property--location {
        margin: 0;
        padding: 0;
    }

    .property--type {
        font-weight: bold;
        line-height: 20px;
        margin: 0;
        padding: 0;
    }

    .property--amenity {
        display: flex;
        justify-content: space-between;
        padding: 0 5px;
        margin-top: 12px;
    }

    .property--amenity span {
        color: red;
        font-size: 15px;
        margin-right: 8px;
    }
</style>
