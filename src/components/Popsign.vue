<template>
  <div>
    <a-button
      id="show-btn"
      style="background: #FFA500; border-radius: 10px;"
      @click="showModal"
      href="#"
    >
      <div style="color: black">Sign In</div>
    </a-button>
    <div class="asd">
      <b-modal
        ref="my-modal"
        body-bg-variant="light"
        hide-header
        hide-footer
        title="Login"
        style="body-radius: 5rem"
        id="modal"
        dialogClassName="border-radius-2"
      >
        <div>
          <button type="button" class="close mt-1 mr-1" aria-label="Close" @click="hideModal">
            <span aria-hidden="true">&times;</span>
          </button>
        </div>
        <!-- <div class="modal-dialog"> -->
        <!-- <div class="modal-content"> -->
        <!-- <div class="modal-backdrop"> -->
        <h1>Daftar</h1>
        <div class="d-block">
          <form ref="form" variant="dark" @submit.stop.prevent="handleSubmit">
            <label>
              <input type="text" id="username" v-model="username" required />
              <div class="label-text">username</div>
            </label>
            <br />
            <label>
              <input type="text" id="email" v-model="email" required />
              <div class="label-text">email</div>
            </label>
            <br />
            <label>
              <input type="password" id="password" v-model="massage" required />
              <div class="label-text">Password</div>
            </label>
          </form>
        </div>
        <div class="text-center">
          <button block @click="hideModal">Sign In</button>
        </div>
        <br />
        <!-- </div> -->
        <!-- </div> -->
        <!-- </div> -->
      </b-modal>
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    showModal() {
      this.$refs["my-modal"].show();
    },
    hideModal() {
      this.$refs["my-modal"].hide();
    },
    toggleModal() {
      // We pass the ID of the button that we want to return focus to
      // when the modal has hidden
      this.$refs["my-modal"].toggle("#toggle-btn");
    }
  }
};
</script>
<style scoped>
.border-radius-2 div {
  border-radius: 2px !important;
}
.close {
  color: black;
}
.modal-content {
  -webkit-border-radius: 10px !important;
  -moz-border-radius: 10px !important;
  border-radius: 10px !important;
}
.modal {
  /* other stuff we already covered */

  width: 600px;
}
h1 {
  padding-left: 10px;
  text-align: center;
  color: black;
}
body {
  background-color: #333333;
  font-family: "Open Sans", Helvetica;
}

form {
  text-align: center;
}

label {
  display: block;
  letter-spacing: 4px;
  padding-top: 30px;
  text-align: center;
}
label .label-text {
  color: #000000;
  cursor: text;
  font-size: 10px;
  line-height: 10px;
  text-transform: uppercase;
  -moz-transform: translateY(-34px);
  -ms-transform: translateY(-34px);
  -webkit-transform: translateY(-34px);
  transform: translateY(-34px);
  transition: all 0.3s;
}
label input {
  background-color: transparent;
  border: 0;
  border-bottom: 2px solid #4a4a4a;
  color: rgb(0, 0, 0);
  font-size: 26px;
  letter-spacing: -1px;
  outline: 0;
  padding: 5px 20px;
  text-align: center;
  transition: all 0.3s;
  width: 200px;
}
label input:focus {
  max-width: 100%;
  width: 210px;
}
label input:focus + .label-text {
  color: #007bff;
  font-size: 13px;
  -moz-transform: translateY(-74px);
  -ms-transform: translateY(-74px);
  -webkit-transform: translateY(-74px);
  transform: translateY(-74px);
}
label input:valid + .label-text {
  font-size: 13px;
  -moz-transform: translateY(-74px);
  -ms-transform: translateY(-74px);
  -webkit-transform: translateY(-74px);
  transform: translateY(-74px);
}

button {
  background-color: #333333;
  border: 2px solid white;
  border-radius: 27px;
  color: white;
  cursor: pointer;
  font-size: 20px;
  margin-top: 20px;
  padding: 15px 30px;
  text-transform: uppercase;
  transition: all 200ms;
}
button:hover,
button:focus {
  background-color: white;
  color: #333333;
  outline: 0;
}
p {
  color: white;
}
</style>