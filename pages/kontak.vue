<template>
  <div class="contact-form">
    <div class="form-section">
      <h2>Hubungi Kami</h2>
      <form @submit.prevent="handleSubmit">
        <div class="form-group">
          <label for="name">Name *</label>
          <input
            type="text"
            id="name"
            v-model="formData.name"
            required
            placeholder="Enter your name"
          />
        </div>
        <div class="form-group">
          <label for="email">E-Mail *</label>
          <input
            type="email"
            id="email"
            v-model="formData.email"
            required
            placeholder="Enter your email"
          />
        </div>
        <div class="form-group">
          <label for="subject">Subject *</label>
          <input
            type="text"
            id="subject"
            v-model="formData.subject"
            required
            placeholder="Enter subject"
          />
        </div>
        <div class="form-group">
          <label for="message">Message *</label>
          <textarea
            id="message"
            v-model="formData.message"
            required
            placeholder="Enter your message"
          ></textarea>
        </div>
        <button type="submit" class="submit-button">Submit</button>
      </form>
    </div>
    <div class="services-section">
      <h2>Layanan yang Kami Tawarkan</h2>
      <ul>
        <li>
          <input type="checkbox" id="website" v-model="services.fullWebsite" />
          <label for="website">Full Website</label>
        </li>
        <li>
          <input
            type="checkbox"
            id="digital-yearbook"
            v-model="services.digitalYearbook"
          />
          <label for="digital-yearbook">Buku Tahunan Digital</label>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      formData: {
        name: "",
        email: "",
        subject: "",
        message: "",
      },
      services: {
        fullWebsite: false,
        digitalYearbook: false,
      },
    };
  },
  methods: {
    handleSubmit() {
      console.log("Form Data:", this.formData);
      console.log("Selected Services:", this.services);
      alert("Form submitted successfully!");
    },
  },
};
</script>

<style scoped>
.contact-form {
  display: flex;
  justify-content: space-between;
  padding: 20px;
  background-color: #1c1c1c;
  color: white;
}

.form-section,
.services-section {
  width: 45%;
}

h2 {
  margin-bottom: 20px;
}

.form-group {
  margin-bottom: 15px;
}

label {
  display: block;
  margin-bottom: 5px;
}

input,
textarea {
  width: 100%;
  padding: 10px;
  margin-bottom: 10px;
  border: 1px solid #ccc;
  border-radius: 5px;
}

.submit-button {
  padding: 10px 20px;
  background-color: #00c2c2;
  border: none;
  color: white;
  border-radius: 5px;
  cursor: pointer;
}

.submit-button:hover {
  background-color: #00a0a0;
}

ul {
  list-style: none;
  padding: 0;
}

li {
  margin-bottom: 10px;
}

input[type="checkbox"] {
  margin-right: 10px;
}
</style>