<template>
  <div class="q-px-xs q-pb-lg">
    <q-card flat bordered class="my-card">
      <q-card-section>
        <q-skeleton v-if="!v" />
        <div class="text-h6" v-else>
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
        <q-skeleton v-if="!v" />
        <div id="qcard-text" v-else>Domínio</div>

        <template>
          <q-tooltip
            content-class="bg-grey-10"
            content-style="font-size: 13px;"
            anchor="top middle"
            self="bottom middle"
            :offset="[10, 10]"
          >
            Domínio é obrigatório, é possível utilizar um já registrado ou fazer
            um novo registro.
          </q-tooltip>
        </template>
      </q-card-section>

      <q-separator inset />

      <q-card-section class="q-pt-none">
        <q-skeleton v-if="!v" />
        <div id="qcard-text" v-else>Hospedagem de site</div>
        <template>
          <q-tooltip
            content-class="bg-grey-10"
            content-style="font-size: 13px;"
            anchor="top middle"
            self="bottom middle"
            :offset="[10, 10]"
          >
            Hospedagem do site, emails e domínio, porque criamos sites apenas em
            nossos servidores.
          </q-tooltip>
        </template>
      </q-card-section>

      <q-separator inset />

      <q-card-section class="q-pt-none">
        <q-skeleton v-if="!v" />
        <div id="qcard-text" v-else>Criação do site</div>
        <template>
          <q-tooltip
            content-class="bg-grey-10"
            content-style="font-size: 13px;"
            anchor="top middle"
            self="bottom middle"
            :offset="[10, 10]"
          >
            Incluso criação de até 6 páginas para o site com o conteúdo enviado.
          </q-tooltip>
        </template>
      </q-card-section>

      <q-separator inset />

      <q-card-section class="q-pt-none">
        <q-skeleton v-if="!v" />
        <div id="qcard-text" v-else>Configuração do sistema online</div>
        <template>
          <q-tooltip
            content-class="bg-grey-10"
            content-style="font-size: 13px;"
            anchor="top middle"
            self="bottom middle"
            :offset="[10, 10]"
          >
            Incluso configuração do sistema online com o conteúdo enviado.
          </q-tooltip>
        </template>
      </q-card-section>

      <q-separator inset />

      <q-card-section class="q-pt-none">
        <q-skeleton v-if="!v" />
        <div id="qcard-text" v-else>Certificado Segurança SSL</div>
        <template>
          <q-tooltip
            content-class="bg-grey-10"
            content-style="font-size: 13px;"
            anchor="top middle"
            self="bottom middle"
            :offset="[10, 10]"
          >
            Com o certificado de segurança SSL os usuários do site serão
            informados que o site é seguro.
          </q-tooltip>
        </template>
      </q-card-section>

      <q-separator inset />

      <q-card-section class="q-pt-none">
        <q-skeleton v-if="!v" />
        <div id="qcard-text" v-else>Treinamento</div>
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
        <q-skeleton v-if="!v" />
        <div id="qcard-text" v-else>Suporte</div>
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
        <q-skeleton v-if="!v" />
        <div id="qcard-text" style="color: white;" v-else>
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
            Após 12 meses do pedido a renovação do serviço é anual, para manter
            todos os serviços online. No cartão de crédito em até 12xR$62,45.
          </q-tooltip>
        </template>
      </q-card-section>

      <q-separator inset />

      <q-card-section class="q-pt-none bg-indigo">
        <q-skeleton v-if="!v" />
        <div id="qcard-text" style="color: white;" v-else>
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
            Esse valor será pago apenas no ato do pedido e inclui 1 ano de
            serviço. No cartão de crédito em até 12xR$104,12.
          </q-tooltip>
        </template>
      </q-card-section>

      <q-separator inset />

      <q-card-section class="q-pt-none bg-indigo">
        <q-skeleton v-if="!v" />
        <div id="qcard-text" style="color: white;" v-else>
          Boleto bancário, cartão de crédito em até 12x, Paypal, Débito,
          Transferência ou Criptomoedas.
        </div>
      </q-card-section>

      <q-separator inset />

      <q-card-section class="q-pt-none">
        <q-skeleton v-if="!v" />
        <div id="qcard-text" v-else>
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
</template>

<style></style>

<script>
export default {
  data() {
    return {
      //Placeholder para verificação de carregamento de algum elemento
      v: true
    };
  },
  name: "barraLateral"
};
</script>
