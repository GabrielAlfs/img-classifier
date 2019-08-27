<template>
  <v-row align="center" justify="center">
    <v-img
      :src="imgUrl"
      lazy-src="https://picsum.photos/id/11/100/60"
      aspect-ratio="1"
      max-width="300"
      max-height="300"
    >
      <template v-slot:placeholder>
        <v-row
          class="fill-height ma-0"
          align="center"
          justify="center"
        >
          <v-progress-circular indeterminate color="blue darken-3"></v-progress-circular>
        </v-row>
      </template>
    </v-img>
  </v-row>
</template>

<script>
export default {
  name: 'previewImage',
  props: ['imgUrl'],
};
</script>

<style>

</style>
