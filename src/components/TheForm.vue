<template>
  <div class="row w-100 my-5 d-flex justify-center">
    <div class="my-5 col-lg-5 col-md-10 col-12">
      <!-- <form name="contact" method="POST" netlify>
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
    </form> -->

      <form id="contattaci" class="pt-5 bg-white flex flex-col justify-center">
        <figure class="flex justify-center">
          <img :src="img" alt="logo_form" />
        </figure>
        <div>
          <h3 class="font-semibold text-2xl mb-5 text-center">
            Compila il form e verrai ricontattato al più presto.
          </h3>
        </div>
        <div class="mb-6">
          <label for="name" class="block mb-2 text-sm font-medium"
            >Nominativo*</label
          >
          <input
            type="text"
            id="name"
            class="bg-gray-50 border border-gray-300 text-sm rounded-lg block w-full p-2.5"
            placeholder="Inserisci nome e cognome."
            required
          />
        </div>
        <div class="mb-6">
          <label for="email" class="block mb-2 text-sm font-medium"
            >Email*</label
          >
          <input
            type="email"
            id="email"
            class="bg-gray-50 border border-gray-300 text-sm rounded-lg block w-full p-2.5"
            placeholder="Inserisci la tua e-mail."
            required
          />
        </div>
        <div class="mb-6 flex flex-col">
          <label for="testo" class="block mb-2 text-sm font-medium"
            >Testo*</label
          >
          <textarea
            class="self-center bg-gray-50 border border-gray-300 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5 dark:border-gray-600 dark:placeholder-gray-400 dark:focus:ring-blue-500 dark:focus:border-blue-500"
            name="testo"
            placeholder="Come possiamo aiutarti?"
            id=""
            cols="35"
            rows="7"
            required
          ></textarea>
          <!-- <input
            type="password"
            id="password"
            class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5 dark:border-gray-600 dark:placeholder-gray-400 dark:focus:ring-blue-500 dark:focus:border-blue-500"
            required
          /> -->
        </div>
        <HomeButton class="bottone" content="Invia" type="submit" />
      </form>
    </div>
  </div>
</template>

<script>
import logoForm from "@/assets/img/logoform-removebg-preview.png";
import HomeButton from "./HomeButton.vue";

export default {
  data() {
    return {
      img: logoForm,
    };
  },
  components: {
    HomeButton,
  },
};
</script>

<style scoped>
figure {
  margin-top: -3rem !important;
}
img {
  height: 12.75rem;
  width: 12.75rem;
  /* margin-left: -1rem; */
}
label {
  width: 70%;
  margin: 0 auto;
}
input {
  border-radius: 25px;
  width: 70%;
  height: 5%;
  margin: 0 auto;
}
textarea {
  width: 70%;
}
form {
  border: inherit;
  padding-bottom: 5rem !important;
  border-radius: 20px;
  box-shadow: rgba(255, 255, 255, 0.1) 0px 1px 1px 0px inset,
    rgba(50, 50, 93, 0.25) 0px 50px 100px -20px,
    rgba(0, 0, 0, 0.3) 0px 30px 60px -30px;
}
.bottone {
  margin: 0 auto;
}
</style>
