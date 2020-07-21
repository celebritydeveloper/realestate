<template>
  <nav class="navbar fixed-top navbar-expand-lg py-3">
        <router-link to="/" class="navbar-brand brand-logo mr-5"><img src="../assets/images/oak-express.png" alt=""></router-link>
            <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>

        <div class="collapse navbar-collapse" id="navbarSupportedContent">
            <ul class="navbar-nav mr-auto flex align-items-center">

                <li class="nav-item active px-3">
                    <router-link to="/">Home <span class="sr-only">(current)</span></router-link>
                </li>
                <li class="nav-item dropdown px-3">
                    <router-link to="/properties" class="nav-link dropdown-toggle" id="navbarDropdown" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">Buy </router-link>
                    <div class="dropdown-menu" aria-labelledby="navbarDropdown">
                        <router-link to="/properties" class="dropdown-item">Property</router-link>
                        <router-link to="/" class="dropdown-item">Land</router-link>
                    <div class="dropdown-divider"></div>
                        <router-link to="/" class="dropdown-item">Property</router-link>
                    </div>
                </li>
                <li class="nav-item dropdown px-3">
                        <router-link to="/" class="nav-link dropdown-toggle" id="navbarDropdown" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">Rent </router-link>
                    <div class="dropdown-menu" aria-labelledby="navbarDropdown">
                        <router-link to="/" class="dropdown-item">Property</router-link>
                        <router-link to="/" class="dropdown-item">Land</router-link>
                    <div class="dropdown-divider"></div>
                        <router-link to="/" class="dropdown-item">Property</router-link>
                    </div>
                </li>
            </ul>
            <ul class="navbar-nav d-flex justify-content-between align-items-center">
                <li class="nav-item px-3">
                    <router-link to="/login">Login</router-link>
                </li>
                <li class="nav-item px-3">
                    <router-link to="/register" class="nav-link button button-brown btn-lg text-white">Create Account</router-link>
                </li>
            </ul>
        </div>
    </nav>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
    .navbar {
        background: rgba(243, 243, 243, 0.6);
    }
    .brand-logo img {
        height: auto;
        width: 90px;
    }

    .brown {
        color: brown;
    }
</style>