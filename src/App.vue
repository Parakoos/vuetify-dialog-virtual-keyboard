<template>
  <div class="page">
    <v-switch v-model="fullscreen" label="Full Screen" />
    <v-dialog v-model="showDialog" :fullscreen="fullscreen">
      <template #activator="{ props }">
        <v-btn color="primary" v-bind="props">Open Dialog</v-btn>
      </template>
      <v-card>
        <v-card-title>Some Header</v-card-title>
        <v-card-text>
          <v-text-field v-model="name" label="Name" autofocus />
          <v-switch v-model="fullscreen" label="Full Screen" />
        </v-card-text>
        <v-card-actions>
          <v-btn @click="showDialog = false">Close</v-btn>
        </v-card-actions>
      </v-card>
    </v-dialog>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue'

const showDialog = ref(false)
const name = ref('')
const fullscreen = ref(false)
</script>
