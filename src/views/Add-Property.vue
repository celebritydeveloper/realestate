<template>
  <div>
      <Nav />
      <div class="container body mx-auto">
          <div class="row">
              <div class="col-xm-12 col-sm-12 col-md-12 col-lg-12 col-xl-12 d-flex justify-content-center align-items-center">
                  <form action="" class="mb-5" style="width: 35rem;">
                    <div class="card" >
                        <img src="https://via.placeholder.com/120" class="card-img-top" height="320"  alt="...">
                        <div class="card-img-overlay d-flex flex-column justify-content-center align-items-center">
                            <font-awesome-icon class="img-icon" :icon="['fas', 'image']"></font-awesome-icon>
                            <input type="file" class="file-upload-img" style="color:transparent;" placeholder="Hello" name="" id="">
                        </div>
                        <div class="card-body">
                            <div class="form-row">
                                <div class="form-group col-md-6">
                                    <label for="inputEmail4">Property Type</label>
                                    <input type="email" class="form-control" id="inputEmail4">
                                </div>
                                <div class="form-group col-md-6">
                                    <label for="inputPassword4">Price</label>
                                    <input type="text" class="form-control" id="inputPassword4">
                                </div>
                                <div class="form-group col-md-4">
                                    <label for="inputPassword4">Bedroom</label>
                                    <select class="form-control">
                                        <option>1</option>
                                        <option>2</option>
                                        <option>3</option>
                                        <option>4</option>
                                    </select>
                                </div>
                                <div class="form-group col-md-4">
                                    <label for="inputPassword4">Bathroom</label>
                                    <select class="form-control">
                                        <option>1</option>
                                        <option>2</option>
                                        <option>3</option>
                                        <option>4</option>
                                    </select>
                                </div>
                                <div class="form-group col-md-4">
                                    <label for="inputPassword4">Bedroom</label>
                                    <select class="form-control">
                                        <option>Default select</option>
                                    </select>
                                </div>
                                <div class="form-group col-md-12">
                                    <label for="exampleFormControlTextarea1">Description</label>
                                    <textarea class="form-control" id="exampleFormControlTextarea1" rows="3"></textarea>
                                </div>
                                <div class="form-group col-md-12">
                                    <label for="inputEmail4">Location</label>
                                    <input type="text" class="form-control" id="inputEmail4">
                                </div>                                
                            </div>
                            <div class="form-row">
                                <div class="form-group col-md-3">
                                    <div class="custom-control custom-checkbox">
                                        <input type="checkbox" class="custom-control-input" id="customCheck1">
                                        <label class="custom-control-label" for="customCheck1">Parking</label>
                                    </div>
                                </div>
                                <div class="form-group col-md-3">
                                    <div class="custom-control custom-checkbox">
                                        <input type="checkbox" class="custom-control-input" id="customCheck2">
                                        <label class="custom-control-label" for="customCheck2">Kitchen</label>
                                    </div>
                                </div>
                                <div class="form-group col-md-3">
                                    <div class="custom-control custom-checkbox">
                                        <input type="checkbox" class="custom-control-input" id="customCheck3">
                                        <label class="custom-control-label" for="customCheck3">Water</label>
                                    </div>
                                </div>
                                <div class="form-group col-md-3">
                                    <div class="custom-control custom-checkbox">
                                        <input type="checkbox" class="custom-control-input" id="customCheck4">
                                        <label class="custom-control-label" for="customCheck4">Balcony</label>
                                    </div>
                                </div>
                            </div>
                            <div class="mx-auto d-flex justify-content-center mt-4">
                                <button type="submit" class="button button-brown text-white btn-lg mb-2 mx-auto">Add Property</button>
                            </div>
                            
                        </div>
                    </div>
                </form>
              </div>
          </div>
      </div>
  </div>
</template>

<script>
import Nav from '../components/Nav';
export default {
    components: {
        Nav,
    }
}
</script>

<style scoped>

    .card-img-overlay {
        height: 55%;
    }

    input.file-upload-img {
        background-color: none;
        box-shadow: none;
        outline: 0;
    }

    .file-upload-img {
        border: none;
    }
    .file-upload-img::-webkit-file-upload-button {
        border: none;
        content: '';
        visibility: hidden;
    }

    .file-upload-img::before {
        color: rgb(88, 86, 86);
        content: 'Add a preview image';
        display: block;
        background: rgb(228, 228, 228);
        /* border: 1px solid red; */
        border-radius: 10px;
        margin: 0 auto;
        padding: 1px 5px;
        outline: none;
        white-space: nowrap;
        -webkit-user-select: none;
        cursor: pointer;
        font-weight: 700;
        font-size: 0.9rem;
        text-align: center;
        width: 50%;
    }

    .file-upload-img::after {
        content: '';
    }

    .file-upload-img:hover::before {
        border-color: red;
        outline-color: transparent;
        outline: none;
    }
    .file-upload-img:active::before {
        background: red;
        outline-color: transparent;
        outline: none;
    }

    .img-icon {
        color: #fff;
        font-size: 3.5rem;
        margin-bottom: 1rem;
    }
</style>