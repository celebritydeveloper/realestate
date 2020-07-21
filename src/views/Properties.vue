<template>
    <div>
        <Nav />
        <div class="container-fluid body">
            <p class="h1 mb-4">156 Results  in Uyo</p>
            <SearchForm />
            <div class="row">
                <div class="col-xm-6 col-sm-6 col-md-3 col-lg-12 col-xl-3" v-for="(property, index) in properties" :key="index">
                    <Property :sample="property" />
                </div>
            </div>
            
            <Pagination />
        </div>        
    </div>
</template>

<script>
import Nav from '../components/Nav';
import Property from '../components/Property';
import SearchForm from '../components/SearchForm';
import Pagination from '../components/Pagination';
import bg from '../assets/images/register-bg.jpg';

export default {

    data() {
        return {
            properties: [
                {
                    name: "3 Bedroom flat",
                    location: "Ikot Ekpene Road",
                    image: bg,
                    bed: 3,
                    bath: 4,
                    parking: 2
                },
                {
                    name: "Full Fledged Duplex",
                    location: "Oron Road, Uyo",
                    image: bg,
                    bed: 7,
                    bath: 10,
                    parking: 4
                },
                {
                    name: "One Bedroom Flat",
                    location: "Ikpa Road",
                    image: bg,
                    bed: 1,
                    bath: 1,
                    parking: 1
                },
                {
                    name: "Ware house for storage",
                    location: "Nwaniba Road",
                    image: bg,
                    bed: 0,
                    bath: 0,
                    parking: 3
                },
                {
                    name: "3 Bedroom flat",
                    location: "Ikot Ekpene Road",
                    image: bg,
                    bed: 3,
                    bath: 4,
                    parking: 2
                },
                {
                    name: "Full Fledged Duplex",
                    location: "Oron Road, Uyo",
                    image: bg,
                    bed: 7,
                    bath: 10,
                    parking: 4
                }
            ],
        }
    },

    components: {
        Nav,
        Property,
        SearchForm,
        Pagination,
    }

}
</script>

<style scoped>
    
</style>