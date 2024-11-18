<script setup lang="ts">
import { ref } from 'vue'
import { SPImagePicker } from 'darklordstudios-vue-component-library'

const tileswidget = ref(null)

const selectedImage = ref('')
</script>

<template>
  <div ref="tileswidget" style="border: 2px solid red">
    <img :src="selectedImage" style="width: 1280px; height: 1020px" />
    <SPImagePicker v-model:imagefield="selectedImage" placeholder="Gimme an image doc" />
  </div>
</template>
