<template>
  <q-layout view="lHh Lpr lFf">
    <q-header elevated>
      <q-toolbar>
        <q-btn
          flat
          dense
          round
          @click="leftDrawerOpen = !leftDrawerOpen"
          icon="menu"
          aria-label="Menu"
        />

        <q-toolbar-title>
          Konversi Mata Uang Asing
        </q-toolbar-title>

        <div>Quasar v{{ $q.version }}</div>
      </q-toolbar>
    </q-header>

    <q-drawer
      v-model="leftDrawerOpen"
      show-if-above
      bordered
      content-class="bg-grey-2"
    >
      <q-list>
        <q-item-label header>Pilih Mata Uang</q-item-label>
        <q-item clickable tag="a" target="_blank">
          <q-item-section avatar>
           </q-item-section>
          <q-item-section>
            <q-item-label>Dollar</q-item-label>
            </q-item-section>
        </q-item>

        <q-item clickable tag="a" target="_blank">
          <q-item-section avatar>
            </q-item-section>
          <q-item-section>
            <q-item-label>Riyal</q-item-label>
            </q-item-section>
        </q-item>

        <q-item clickable tag="a" target="_blank">
          <q-item-section avatar>
            </q-item-section>
          <q-item-section>
            <q-item-label>Yen</q-item-label>
            </q-item-section>
        </q-item>

        <q-item clickable tag="a" target="_blank">
          <q-item-section avatar>
            </q-item-section>
          <q-item-section>
            <q-item-label>Ringgit</q-item-label>
            </q-item-section>
        </q-item>

        <q-item clickable tag="a" target="_blank">
          <q-item-section avatar>
            </q-item-section>
          <q-item-section>
            <q-item-label>Yuan</q-item-label>
            </q-item-section>
        </q-item>

        <q-item clickable tag="a" target="_blank">
          <q-item-section avatar>
            </q-item-section>
          <q-item-section>
            <q-item-label>Euro</q-item-label>
            </q-item-section>
        </q-item>
      </q-list>
    </q-drawer>

    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>
export default {
  name: 'MyLayout',

  data () {
    return {
      leftDrawerOpen: false
    }
  }
}
</script>
