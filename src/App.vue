<template>
  <q-layout view="lHh Lpr lFf" class="bg-grey-2">
    <div id="header" class="row q-pa-lg">
      <h4>Solicitando Serviço</h4>
      <p>
        Por favor preencha corretamente os dados do formulário abaixo para ter
        seu pedido aprovado rapidamente. Durante o cadastro é possível registrar
        um novo domínio pago (exemplo: .com.br), utilizar um domínio já
        registrado.
      </p>
    </div>

    <q-page-container>
      <div class="q-pa-lg">
        <div class="row">
          <div id="col-start" class="col-12 col-sm-7 col-md-8">
            <formulario />
          </div>

          <div id="col-end" class="col-12 col-sm-5 col-md-4">
            <barraLateral />
          </div>
        </div>
      </div>

      <footer class="q-pa-md bg-grey-4">
        <div id="footer">
          Você está em um ambiente seguro | <a href="">Suporte</a><br />
          Site protegido pelo Google reCAPTCHA.
          <a href="">Políticas de Privacidade</a> e
          <a href="">Termos de Serviço</a> aplicados.<br />
          © Link Nacional desde 2004 | Brasil | Todos os direitos reservados
        </div>
      </footer>
    </q-page-container>
  </q-layout>
</template>

<script>
import formulario from "./components/Formulario.vue";
import barraLateral from "./components/BarraLateral.vue";

export default {
  components: {
    formulario,
    barraLateral
  },

  data() {
    return {
      password: "",
      isPwd: true,

      email: ""
    };
  },
  name: "LayoutDefault"
};
</script>

<style>
@import "./styles/indexStyle.css";
</style>
