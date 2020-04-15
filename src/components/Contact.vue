<template>
  <div class="content">
    <h1>Contato</h1>
    <p>
      Você entrar em contato comigo pelo
      <a class="no-underline" href="https://t.me/fbior" target="_blank">
        <v-hover>
          <v-icon
            @mouseover="next_active = true"
            @mouseout="next_active = false"
            slot-scope="{ hover }"
            :class="`${hover? 'icon-active': 'icon-inactive'}`"
          >fab fa-telegram</v-icon>
        </v-hover>
      </a> ou pelo endereço de e-mail
      <code class="inline">fabio_rolim@hotmail.com</code>
    </p>
    <BaseFooter
      :items="[
                {value: 'Home', url: '/'},
                {value: 'Contact', url: '/contact'},
                {value: 'Subscribe', url: '/subscribe'}]"
    ></BaseFooter>
  </div>
</template>

<script>
import BaseFooter from "@/components/BaseFooter.vue";

export default {
  name: "Home",

  components: {
    BaseFooter
  }
};
</script>

<style scoped>
</style>
