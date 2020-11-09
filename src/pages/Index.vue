<template>
  <q-page class="flex flex-center">
    <div class="flex flex-center text-left">
    <p><strong>Country flags (11):</strong></p>
    <div class="fit row wrap justify-center items-center content-start">
      <country-flag
        style="border-radius: 12px;"
        v-for="(country, index) in countries"
        :key="index"
        :country="country"
        size="big"
      />
    </div>
  </div>
  </q-page>
</template>

<script>
export default {
  name: 'PageIndex',
  data() {
    return {
      countries: ['gb', 'fr', 'es', 'it', 'ru', 'pt', 'de', 'pl', 'kr', 'jp', 'cn'],
    };
  },
};
</script>
