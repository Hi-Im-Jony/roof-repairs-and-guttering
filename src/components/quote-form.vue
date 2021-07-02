<template>
  <div id="form-container">
    <h1>Get A Free Qoute Today</h1>
    <form
      name="quote-form"
      method="POST"
      data-netlify="true"
      data-netlify-honeypot="bot-field"
      @submit.prevent="handleSubmit"
    >
      <input type="hidden" name="form-name" value="quote-form" />

      <h2 id="form-title">
        {{ formMessage }}
      </h2>
      <div class="input-container">
        <v-text-field
          v-model="form.name"
          name="name"
          label="Your Name"
          required
          color="aliceblue"
          dark
        ></v-text-field>
        <v-select
          v-model="form.service"
          name="service"
          :items="items"
          label="Service Required"
          required
          color="aliceblue"
          dark
        ></v-select>

        <v-text-field
          v-model="form.phone"
          name="phone"
          label="Phone"
          required
          color="aliceblue"
          dark
        ></v-text-field>

        <v-text-field
          v-model="form.email"
          name="email"
          label="E-mail"
          required
          color="aliceblue"
          dark
        ></v-text-field>

        <v-textarea
          v-model="form.message"
          name="message"
          label="Message"
          color="aliceblue"
          dark
        ></v-textarea>
      </div>
      <div>
        <button type="submit">Send</button>
      </div>
    </form>
  </div>
</template>

<script>
export default {
  name: "quoteForm",
  props: ["formMessage"],
  data: () => ({
    form: {
      name: "",
      phone: "",
      email: "",
      message: "",
    },
    items: ["Roofing", "Guttering", "Chimney"],
  }),
  methods: {
    encode(data) {
      return Object.keys(data)
        .map(
          (key) => encodeURIComponent(key) + "=" + encodeURIComponent(data[key])
        )
        .join("&");
    },
    handleSubmit() {
      fetch("/", {
        method: "post",
        headers: {
          "Content-Type": "application/x-www-form-urlencoded",
        },
        body: this.encode({
          "form-name": "quote-form",
          ...this.form,
        }),
      });
      then(() => {
        this.$router.push("thanks");
      }).catch(() => {
        this.$router.push("404");
      });
    },
  },
};
</script>

<style scoped>
#form-container {
  width: 25%;
  min-width: 270px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  margin: 10px;
  text-align: center;
  color: #dc143c;
}
form {
  background: rgba(11, 19, 43, 0.836);
  color: aliceblue;
  width: 400px;
  padding: 20px;
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
}
.input-container {
  width: 90%;
}

@media (max-width: 720px) {
  form {
    width: 95%;
    max-width: 400px;
  }
}
</style>
