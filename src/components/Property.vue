<template>
  <section class="py-3">
                <div>
                    <div class="card property--card rounded">
                        <img src="../assets/images/property-1.jpg" class="card-img-top rounded property-img" height="320" alt="...">
                        <div class="card-footer mx-auto rounded property--footer position-relative">
                            <p class="property--location">{{sample.location}}</p>
                            <p class="h5 property--type">{{sample.name}}</p>
                            <div class="property--amenity">
                                <span>
                                    <font-awesome-icon icon="couch"></font-awesome-icon>
                                    {{sample.bed}} Bed</span>
                                <span>
                                    <font-awesome-icon icon="bath"></font-awesome-icon>
                                    {{sample.bath}} Bath</span>
                                <span>
                                    <font-awesome-icon icon="car"></font-awesome-icon>
                                   {{sample.parking}}</span>
                            </div>
                        </div>
                    </div>
                </div>
             
        </section>
</template>

<script>

export default {
    data() {
        return {
             
        }
    },

    props: [
        "sample"
    ],

    components: {
    }
}
</script>

<style scoped>
    .property--card {
        border: none;
        cursor: pointer;
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
        color: rgb(189,139,40);
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
        color: rgb(189,139,40);
        font-size: 15px;
        margin-right: 8px;
    }
</style>