<template>
  <div>
    <q-card class="my-card" flat bordered>
      <q-item>
        <q-item-section>
          <q-item-label></q-item-label>
          <q-item-label caption> FIX HERE </q-item-label>
        </q-item-section>
      </q-item>

      <q-separator />

      <q-card-section horizontal>
        <q-card-section>
          <q-tabs v-model="tab" vertical class="text-primary">
            <q-tab name="profile" icon="contact_mail" label="Profile" />
            <q-tab name="account" icon="account_box" label="Account" />
            <q-tab name="preferences" icon="movie" label="Preferences" />
          </q-tabs>
        </q-card-section>

        <q-separator vertical />

        <q-card-section class="col-10">
          <q-tab-panels v-model="tab" swipeable vertical>
            <q-tab-panel name="account">
              <div class="q-mb-md">
                <q-input label="Your name *" v-model="val"></q-input>
              </div>
            </q-tab-panel>
            <q-tab-panel name="profile">
              <div class="q-mb-md">
                <q-input label="Your name *" v-model="val"></q-input>
              </div>
            </q-tab-panel>
            <q-tab-panel name="preferences">
              <div class="q-mb-md">Preferences</div>
            </q-tab-panel>
          </q-tab-panels>
        </q-card-section>
      </q-card-section>
    </q-card>
  </div>
</template>

<script lang="ts" setup>
const tab = ref("profile");
const val = ref("profile");
</script>

<style></style>
