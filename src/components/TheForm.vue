<template>
  <div class="padre">
    <form name="contact" method="POST" netlify>
      <figure>
        <img :src="img" alt="logo_form" />
      </figure>
      <h3>Compila il form e verrai ricontattato al più presto</h3>
      <p>
        <label>Nome* <input type="text" name="name" /></label>
      </p>
      <p>
        <label>Email* <input type="email" name="email" /></label>
      </p>
      <p>
        <label>Numero di telefono <input type="text" name="name" /></label>
      </p>
      <p>
        <label
          >Testo* <textarea name="body" id="" cols="30" rows="10"></textarea>
        </label>
      </p>
    </form>
  </div>
</template>

<script>
import logoForm from "@/assets/img/logoform-removebg-preview.png";

export default {
  data() {
    return {
      img: logoForm,
    };
  },
};
</script>

<style></style>
