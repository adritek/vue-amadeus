<template>
  <form @submit.prevent="submitForm">
    <div>
      <label for="firstName">First Name:</label>
      <input type="text" id="firstName" v-model="formData.firstName" required />
    </div>

    <div>
      <label for="lastName">Last Name:</label>
      <input type="text" id="lastName" v-model="formData.lastName" required />
    </div>

    <div>
      <label for="email">Email:</label>
      <input type="email" id="email" v-model="formData.email" required />
    </div>

    <div>
      <label for="phone">Phone:</label>
      <input type="phone" id="phone" v-model="formData.phone"  />
    </div>

    <div>
      <label for="comments">Comments:</label>
      <input type="text" id="comments" v-model="formData.comments" required />
    </div>

    <button type="submit">Submit</button>
  </form>
</template>

<script>
  export default {
    data() {
      return {
        formData: {
          firstName: '',
          lastName: '',
          email: '',
          phone: '',
          comments: ''
        }
      }
    },
    methods: {
      submitForm() {
      console.log(this.formData);
      }
   }
  }
</script>