<template>
<q-layout>
<!-- Header -->
  <q-toolbar slot="header">
    <q-btn flat @click="$refs.layout.toggleLeft()">
      <q-icon name="menu" />
    </q-btn>
    <q-toolbar-title>
      Lunch Tips
      <span slot="subtitle">Ask me ,Tips you ~ </span>
    </q-toolbar-title>
    <!-- <q-btn flat @click="$refs.layout.toggleRight()">
      <q-icon name="menu" />
    </q-btn> -->
  </q-toolbar>

<!-- -->
<div>
  <input v-model="parentMsg">
  <br>
  <div v-bind:my-message="parentMsg"></div>
</div>

</q-layout>
</template>
<script>
import {
  // dom,
  // event,
  // openURL,
  QLayout,
  QBtn,
  QIcon,
  QToolbar,
  QToolbarTitle,
  QSearch,
  QField
} from 'quasar'

export default {
  components: {
    QLayout,
    QBtn,
    QIcon,
    QToolbar,
    QToolbarTitle,
    QSearch,
    QField
  }
}
</script>

<style>

</style>
