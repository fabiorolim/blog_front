<template>
  <div>
    <h1>Sobre</h1>
    <img
      src="https://avatars0.githubusercontent.com/u/7581320?s=460&u=7ec8b48466d7ed1bd44baf1b2131b8ef684733b2&v=4"
      style=" width: 90px; border-radius: 50%;"
    />
    <p>
      Eu me chamo Fábio Rolim, sou Analista de Sistemas de formação acadêmica, apaixonado e eterno
      estudante do mundo da tecnologia e computadores, sobretudo, desenvolvimento de software. :)
    </p>
    <p>
      Atualmente sou professor do Ensino Básico Técnico e Tencológico, atuando no eixo Informática e
      Comunicação no IFPI (Instituto Federal do Piauí) Campus Oeiras.
      Também oriento alunos de times de desenvolvimento de softwares no NDS (Núcleo de Desenvolvimento de
      Software)
      do IFPI - Oeiras.
    </p>
    <p>
      Você pode me encontrar no
      <a
        class="no-underline"
        href="https://github.com/fabiorolim"
        target="_blank"
      >
        <v-hover>
          <v-icon
            @mouseover="next_active = true"
            @mouseout="next_active = false"
            slot-scope="{ hover }"
            :class="`${hover? 'icon-active': 'icon-inactive'}`"
          >fab fa-github</v-icon>
        </v-hover>
      </a>.
    </p>
  </div>
</template>

<script>
export default {
  name: "About"
};
</script>

<style>
.custom-btn::before {
  color: transparent;
}

.custom-btn:hover {
  color: #0088cd;
  min-width: 0;
}

.no-underline {
  background-image: none !important;
}

.column {
  float: left;
  width: 33%;
  padding: 10px;
  height: 50%;
}

/* Clear floats after the columns */
.row:after {
  content: "";
  display: table;
  clear: both;
}

.about-list {
  padding-left: 12px;
}

@media (min-width: 320px) and (max-width: 600px) {
  #cols .column {
    width: 100%;
  }
}
</style>
