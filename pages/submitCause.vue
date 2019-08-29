<template>
  <div id="banner">
    <div class="row">
      <div class="col-lg-12 text-center">
        <h2 class="sub">
          Submit Your Cause for Consideration
        </h2>
        <h5>
          Add your cause, identify yourself and give us as much infomation as
          possible for consideration.
        </h5>
        <p>
          For Now...Anything goes..
        </p>
      </div>
    </div>
    <div id="form-stuff">
      <b-form-group id="input-group-1" label="Cause Title:" label-for="input-2">
        <b-form-input
          id="input-2"
          v-model="form.name"
          required
          placeholder="Title Your Cause"
        ></b-form-input>
      </b-form-group>

      <!-- <b-form-group
        id="input-desc"
        label="Cause Description:"
        label-for="input-2"
      >
        <b-form-input
          id="input-desc-2"
          v-model="form.name"
          required
          placeholder="Describe Your Cause"
        ></b-form-input>
      </b-form-group> -->
      <div>
        <b-form-group
          id="input-desc"
          label="Cause Description:"
          label-for="textDesc"
        >
          <b-form-textarea
            id="textDesc"
            v-model="form.textDesc"
            placeholder="Enter Your Cause Description..."
            rows="5"
            max-rows="12"
          ></b-form-textarea>
        </b-form-group>
        <pre class="mt-3 mb-0">{{ text }}</pre>
      </div>

      <b-form-group id="input-name" label="Your Name:" label-for="input-2">
        <b-form-input
          id="input-2"
          v-model="form.name"
          required
          placeholder="Enter name"
        ></b-form-input>
      </b-form-group>

      <b-form v-if="show" @submit="onSubmit" @reset="onReset">
        <b-form-group
          id="input-email"
          label="Email address:"
          label-for="input-1"
          description="We'll never share your email with anyone else."
        >
          <b-form-input
            id="input-1"
            v-model="form.email"
            type="email"
            required
            placeholder="Enter email"
          ></b-form-input>
        </b-form-group>

        <b-form-group
          id="input-wallet"
          v-model="form.EthWallet"
          label="Your ETH Wallet Address:"
          label-for="input-2"
        >
          <b-form-input
            id="input-2"
            v-model="form.walletID"
            required
            placeholder="Enter name"
          ></b-form-input>
        </b-form-group>

        <div id="image-choose">
          <h5>Upload an Image for your Cause</h5>
          <!-- Styled -->
          <b-form-file
            v-model="file"
            :state="Boolean(file)"
            placeholder="Choose a file..."
            drop-placeholder="Drop file here..."
            label="Upload a Cause Image"
            label-for="image-choose"
          ></b-form-file>
          <div class="mt-3">Selected file: {{ file ? file.name : '' }}</div>
        </div>

        <div id="avatar-choose">
          <h5>Upload an Image for your Avatar</h5>
          <!-- Styled -->
          <b-form-file
            v-model="fileAva"
            :state="Boolean(fileAva)"
            placeholder="Choose a file..."
            drop-placeholder="Drop file here..."
            label="Upload a Cause Image"
            label-for="image-choose"
          ></b-form-file>
          <div class="mt-3">
            Selected file: {{ fileAva ? fileAva.name : '' }}
          </div>
        </div>

        <div>
          <b-button type="submit" variant="primary">Submit</b-button>
          <b-button type="reset" variant="danger">Reset</b-button>
        </div>
      </b-form>
    </div>

    <b-card class="mt-3" header="Form Data Result">
      <pre class="m-0">{{ form }}</pre>
      <pre class="m-0">{{ file }}</pre>
      <pre class="m-0">{{ fileAva }}</pre>
      <pre class="m-0">{{ textDesc }}</pre>
    </b-card>
  </div>
</template>

<script>
export default {
  data() {
    return {
      file: {
        file: null,
        file2: null
      },
      fileAva: {
        file: null,
        file2: null
      },
      form: {
        email: '',
        name: '',
        walletId: '',
        food: null,
        checked: [],
        descText: '',
        EthWallet: ''
      },
      foods: [
        { text: 'Select One', value: null },
        'Carrots',
        'Beans',
        'Tomatoes',
        'Corn'
      ],
      show: true
    }
  },
  methods: {
    onSubmit(evt) {
      evt.preventDefault()
      alert(JSON.stringify(this.form))
    },
    onReset(evt) {
      evt.preventDefault()
      // Reset our form values
      this.form.email = ''
      this.form.name = ''
      this.form.food = null
      this.form.walletId = ''

      this.form.checked = []
      this.file.file = null
      this.fileAva.file = null
      // Trick to reset/clear native browser form validation state
      this.show = false
      this.$nextTick(() => {
        this.show = true
      })
    }
  }
}
</script>

<style scoped>
#banner {
  padding-top: 100px;
  margin-left: 120px;
  margin-right: 120px;
  min-width: 250px;
}

#form-stuff {
  align-content: center;
}
#sub {
  font-size: 36px;
}
#input-group-1 {
  margin-left: 120px;
  margin-right: 120px;
  padding-top: 100px;
  width: 70%;
  align-content: center;
}
#input-name {
  margin-left: 120px;
  margin-right: 120px;
  width: 70%;
}
#input-email {
  margin-left: 120px;
  margin-right: 120px;
  width: 70%;
}
#input-desc {
  margin-left: 120px;
  margin-right: 120px;
  width: 70%;
}
#input-desc-2 {
  height: 300px;
}
#input-wallet {
  margin-left: 120px;
  margin-right: 120px;
  width: 70%;
}
#image-choose {
  margin-left: 120px;
  margin-right: 120px;
  width: 70%;
  padding-bottom: 40px;
  padding-top: 50px;
}
#avatar-choose {
  margin-left: 120px;
  margin-right: 120px;
  width: 70%;
  padding-bottom: 30px;
  padding-top: 30px;
}

/* #textDesc {
  margin-left: 120px;
  margin-right: 120px;
  max-height: 400px;
  width: 70%;
} */
.b-form-group {
  border-radius: 7px;
}
</style>
