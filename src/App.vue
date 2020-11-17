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
            <div class="q-px-xs q-pb-lg">
              <q-card flat bordered class="my-card">
                <q-card-section>
                  <div class="text-h6">
                    Serviços Inclusos

                    <template>
                      <q-badge
                        align="middle"
                        color="grey-8"
                        text-color="grey-11"
                        label="7"
                      />
                    </template>
                  </div>
                </q-card-section>

                <q-card-section class="q-pt-none">
                  <div id="qcard-text">Domínio</div>

                  <template>
                    <q-tooltip
                      content-class="bg-grey-10"
                      content-style="font-size: 13px;"
                      anchor="top middle"
                      self="bottom middle"
                      :offset="[10, 10]"
                    >
                      Domínio é obrigatório, é possível utilizar um já
                      registrado ou fazer um novo registro.
                    </q-tooltip>
                  </template>
                </q-card-section>

                <q-separator inset />

                <q-card-section class="q-pt-none">
                  <div id="qcard-text">Hospedagem de site</div>
                  <template>
                    <q-tooltip
                      content-class="bg-grey-10"
                      content-style="font-size: 13px;"
                      anchor="top middle"
                      self="bottom middle"
                      :offset="[10, 10]"
                    >
                      Hospedagem do site, emails e domínio, porque criamos sites
                      apenas em nossos servidores.
                    </q-tooltip>
                  </template>
                </q-card-section>

                <q-separator inset />

                <q-card-section class="q-pt-none">
                  <div id="qcard-text">Criação do site</div>
                  <template>
                    <q-tooltip
                      content-class="bg-grey-10"
                      content-style="font-size: 13px;"
                      anchor="top middle"
                      self="bottom middle"
                      :offset="[10, 10]"
                    >
                      Incluso criação de até 6 páginas para o site com o
                      conteúdo enviado.
                    </q-tooltip>
                  </template>
                </q-card-section>

                <q-separator inset />

                <q-card-section class="q-pt-none">
                  <div id="qcard-text">Configuração do sistema online</div>
                  <template>
                    <q-tooltip
                      content-class="bg-grey-10"
                      content-style="font-size: 13px;"
                      anchor="top middle"
                      self="bottom middle"
                      :offset="[10, 10]"
                    >
                      Incluso configuração do sistema online com o conteúdo
                      enviado.
                    </q-tooltip>
                  </template>
                </q-card-section>

                <q-separator inset />

                <q-card-section class="q-pt-none">
                  <div id="qcard-text">Certificado Segurança SSL</div>
                  <template>
                    <q-tooltip
                      content-class="bg-grey-10"
                      content-style="font-size: 13px;"
                      anchor="top middle"
                      self="bottom middle"
                      :offset="[10, 10]"
                    >
                      Com o certificado de segurança SSL os usuários do site
                      serão informados que o site é seguro.
                    </q-tooltip>
                  </template>
                </q-card-section>

                <q-separator inset />

                <q-card-section class="q-pt-none">
                  <div id="qcard-text">Treinamento</div>
                  <template>
                    <q-tooltip
                      content-class="bg-grey-10"
                      content-style="font-size: 13px;"
                      anchor="top middle"
                      self="bottom middle"
                      :offset="[10, 10]"
                    >
                      Treinamento de como utilizar toda a plataforma do site.
                    </q-tooltip>
                  </template>
                </q-card-section>

                <q-separator inset />

                <q-card-section class="q-pt-none">
                  <div id="qcard-text">Suporte</div>
                  <template>
                    <q-tooltip
                      content-class="bg-grey-10"
                      content-style="font-size: 13px;"
                      anchor="top middle"
                      self="bottom middle"
                      :offset="[10, 10]"
                    >
                      Suporte 24h para dúvida e ajuda com o site.
                    </q-tooltip>
                  </template>
                </q-card-section>

                <q-separator inset />

                <q-card-section class="q-pt-none bg-indigo">
                  <div id="qcard-text" style="color: white;">
                    Após 12 meses <strong> R$749,50 por ano</strong>
                  </div>

                  <template>
                    <q-tooltip
                      content-class="bg-grey-10"
                      content-style="font-size: 13px;"
                      anchor="top middle"
                      self="bottom middle"
                      :offset="[10, 10]"
                    >
                      Após 12 meses do pedido a renovação do serviço é anual,
                      para manter todos os serviços online. No cartão de crédito
                      em até 12xR$62,45.
                    </q-tooltip>
                  </template>
                </q-card-section>

                <q-separator inset />

                <q-card-section class="q-pt-none bg-indigo">
                  <div id="qcard-text" style="color: white;">
                    Total hoje <strong> R$1249,45</strong>
                  </div>

                  <template>
                    <q-tooltip
                      content-class="bg-grey-10"
                      content-style="font-size: 13px;"
                      anchor="top middle"
                      self="bottom middle"
                      :offset="[10, 10]"
                    >
                      Esse valor será pago apenas no ato do pedido e inclui 1
                      ano de serviço. No cartão de crédito em até 12xR$104,12.
                    </q-tooltip>
                  </template>
                </q-card-section>

                <q-separator inset />

                <q-card-section class="q-pt-none bg-indigo">
                  <div id="qcard-text" style="color: white;">
                    Boleto bancário, cartão de crédito em até 12x, Paypal,
                    Débito, Transferência ou Criptomoedas.
                  </div>
                </q-card-section>

                <q-separator inset />

                <q-card-section class="q-pt-none">
                  <div id="qcard-text">
                    <strong>Suporte 24h, todos os dias.</strong><br />
                    Garanta seu site sempre no ar
                  </div>

                  <template>
                    <q-tooltip
                      content-class="bg-grey-10"
                      content-style="font-size: 13px;"
                      anchor="top middle"
                      self="bottom middle"
                      :offset="[10, 10]"
                    >
                      Cadastro e homologação junto a Cielo.
                    </q-tooltip>
                  </template>
                </q-card-section>

                <q-separator inset />
              </q-card>
            </div>
          </div>
        </div>
      </div>
      <!--<HelloWorld />-->
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
// import HelloWorld from './components/HelloWorld.vue';
import formulario from "./components/formulario.vue";

export default {
  components: {
    formulario
  },

  data() {
    return {
      password: "",
      isPwd: true,

      email: ""
    };
  },
  name: "LayoutDefault"

  /* components: {
  HelloWorld
    }, */
};
</script>

<style>
#header {
  justify-content: center;
  margin-left: 15%;
  margin-right: 15%;
  text-align: center;
}

h4 {
  margin-bottom: 3%;
}

h5 {
  margin: 0%;
  padding: 0%;
}

#text-hform {
  color: grey;
  font-size: medium;
}

#footer {
  justify-content: center;
  text-align: center;
  margin-left: 20%;
  margin-right: 20%;
  color: grey;
  font-size: small;
}

#qcard-text {
  font-size: medium;
  padding-top: 1em;

  padding-left: 1em;
}

@media screen and (max-width: 599px) {
  #col-start {
    order: 2;
    padding-bottom: 3%;
    padding-top: 3%;
  }
  #footer {
    justify-content: center;
    text-align: center;
    margin-left: 5%;
    margin-right: 5%;
    font-size: 13px;
    line-height: 2em;
  }
}
</style>
