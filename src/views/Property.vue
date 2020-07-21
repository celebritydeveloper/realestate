<template>
  <div>
      <Nav />
      <div class="container-fluid body">
          <div class="row">
            <div class="col-xm-12 col-sm-12 col-md-7 col-lg-7 col-xl-7">
                <div class="property-top">
                    <div class="property-type">
                        <p class="property-name">3 Bedroom Flat
                            <span class="property-location">Ikpa Road, Uyo</span>
                        </p>
                        <p class="property-price">N200,000</p>
                    </div>
                    <p class="property-status rounded text-center">Sold</p>
                </div>
                <img :src="bg" class="img-fluid" height="" alt="...">
                <div class="container-fluid">
                    <div class="row">
                        <div class="col-xm-4 col-sm-4 col-md-4 col-lg-4 col-xl-4">
                            <font-awesome-icon icon="couch"></font-awesome-icon>
                        </div>
                        <div class="col-xm-4 col-sm-4 col-md-4 col-lg-4 col-xl-4">
                            <font-awesome-icon icon="bath"></font-awesome-icon>
                        </div> 
                        <div class="col-xm-4 col-sm-4 col-md-4 col-lg-4 col-xl-4">
                            <font-awesome-icon icon="car"></font-awesome-icon>
                        </div>   
                    </div>
                    <div class="row">
                        <div class="col-xm-12 col-sm-12 col-md-12 col-lg-12 col-xl-12">
                            Lorem ipsum dolor, sit amet consectetur adipisicing elit. Temporibus vel architecto officia nesciunt ut repudiandae sint at fugiat quia? Quam.
                        </div>   
                    </div>
                </div>
            </div>

            <div class="offset-md-1 col-xm-12 col-sm-12 col-md-4 col-lg-4 col-xl-4">
                <div class="card agent-card rounded flex flex-column justify-content-center align-items-center py-5">
                    <img :src="bg" class="rounded-circle mx-auto" height="110" width="110" alt="...">  
                    <div class="mt-4">
                        <p class="h4">Saviour Essien</p>
                        <p class="h4"></p>
                        <button class="button button-brown btn-lg text-white">Contact Agent</button>
                    </div>
                </div>
            </div>
          </div>
          
      </div>
  </div>
</template>

<script>
import Nav from '../components/Nav';
import bg from '../assets/images/register-bg.jpg';

export default {
    data() {
        return {
            bg,
        }
    },

    components: {
        Nav,
    }
}
</script>

<style scoped>

    .agent-card {
        border: none;
        box-shadow: 2px 3px 15px rgb(226, 226, 226);
    }

    .property-top {
        background: #fff;
        box-shadow: 2px 3px 15px rgb(226, 226, 226);
        padding: 0.3rem 1.2rem;
    }

    .property-type {
        align-items: center;
        display: flex;
        justify-content: space-between;
    }

    .property-name {
        display: flex;
        font-size: 1.6rem;
        flex-direction: column;
        justify-content: space-between;
    }

    .property-location {
        font-size: 1rem;
    }

    .property-price {
        font-size: 1.3rem;
    }

    .property-status {
        background: red;
        width: 10%;
    }

</style>