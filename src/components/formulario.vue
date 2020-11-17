<template>
  <div class="q-px-xs">
    <div class="q-ma-none q-pb-lg">
      <h5>Criar uma conta</h5>
      <br />
      <div id="text-hform">
        Informe um endereço de e-mail válido e uma senha para acompanhar sua
        solicitação online.
      </div>
    </div>
    <q-form @submit="onSubmit" @reset="onReset" class="q-gutter-md">
      <q-input
        filled
        v-model="email"
        type="email"
        label="Seu email"
        hint="Insira um email válido"
      />

      <q-input
        v-model="password"
        filled
        :type="isPwd ? 'password' : 'text'"
        hint="Criar uma senha de acesso"
      >
        <template v-slot:append>
          <q-icon
            :name="isPwd ? 'visibility_off' : 'visibility'"
            class="cursor-pointer"
            @click="isPwd = !isPwd"
          />
        </template>
      </q-input>

      <q-input
        filled
        v-model="phone"
        label="Telefone"
        mask="(##) ##### - ####"
        fill-mask
        hint="Whatsapp ou Telegram"
      />

      <div>
        <q-btn label="Criar conta" type="submit" color="primary" />
        <q-btn
          label="Mais informações"
          type="reset"
          color="primary"
          flat
          class="q-ml-sm"
        />
      </div>
    </q-form>
  </div>
</template>

<style></style>

<script>
export default {
  name: "formulario"
};
</script>
